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

# AWS CLI Most Used Commands

aws s3 sync dist/ s3://2024ana --delete
→ Removed old build files and uploaded your latest Vite dist/ output to the 2024ana bucket.

aws cloudfront create-invalidation --distribution-id E1IRVC5C4GFCAP --paths "/*"
→ Told CloudFront to clear its cache so it will serve the fresh version from S3.


