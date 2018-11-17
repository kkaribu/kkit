# Commands

## modif <name>

Make sure the repository is checked out on a release branch or master.

`<date>` is the current date in YYMMDD format.

```
git checkout -b modif-<date>-<name>
```

Create the necessary files.

```
KKIT-<date>-<name>-AUTHORS.txt
KKIT-<date>-<name>-COMMENTS.txt
KKIT-<date>-<name>-MESSAGE.txt
```

## apply

Read the necessary data from the modif files (the ones that start with *KKIT-*).

Checkout the parent branch.

Copy the tree and merge it in the parent branch.

```
git read-tree -m -u <modif-branch>
```
