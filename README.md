# Git Most Used Commands

This document contains some of the most useful Git commands based on personal experience.

## Listing Remote Branches
To list all remote branches in a Git repository, use the following command:

```sh
git branch -r
```

If you want to see both local and remote branches, use:

```sh
git branch -a
```

## Creating a New Branch
To create a new branch from the current branch:

```sh
git branch <new-branch-name>
```

To switch to the newly created branch immediately, use:

```sh
git checkout -b <new-branch-name>
```

or the newer equivalent:

```sh
git switch -c <new-branch-name>
```

## Viewing Remote Tracking Branches
For more details, such as the remote tracking branches, use:

```sh
git ls-remote --heads origin
```

---
These commands are handy for everyday Git usage. 🚀
