# git_most_used_commands
these are helpful for my personal experience 

To list all remote branches in a Git repository, use the following command:
git branch -r

If you want to see both local and remote branches, use:
git branch -a


To create a new branch from the current branch:
git branch <new-branch-name>

to switch to the newly created branch immediately, use:
git checkout -b <new-branch-name>
or
git switch -c <new-branch-name>

more details, such as the remote tracking branches
git ls-remote --heads origin


