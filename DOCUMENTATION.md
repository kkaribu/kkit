# Documentation

The documentation is a work in progress.

See COMMANDS.md for details about each command.

## Modifying the code

The bring any kind of modification to the code base, a branch must be created. Anything can be commited a modif branch as long as the commits are related to the change being made.

The workflow is the same for small bugfixes, new features, huge refactoring jobs, etc. 

1. Checkout on master or a release branch. If the change will break the API, it **must** be master. 
2. Execute `kkit modif <name>` where `<name>` is the name of the modification.
3. You will automatically get checked out on the new branch.
4. Make commits as necessary.
5. From time to time, keep your modif branch synced with its parent branch (and never with any other branch) with `kkit sync`.
6. Once ready to merge, sync one last time if necessary to make sure that your last commit contains everything that was introduced in the release since the modif branch was created. This is really important and kitt will prevent you to merge if it isn't done.
7. Merge with `kitt apply`.
8. Commit your updated release branch. The modif branch will stay there, but it can be deleted. It should not be reused.

The quality of the commit messages is less important, as everything will be summarized in a single commit at the end.

## Branches

### Master

### Release branches

### Modifications

## Commiting modification

Once