# git local-commits 
## chatgpt 
There is no actual Git command called "git local-commits". However, there are certain Git commands that involve local commits, such as:

1. `git commit`: This command creates a local commit with the changes made to the current branch. It is used after staging changes with `git add`.

2. `git log`: This command displays the log of all commits made to the current branch, including local commits.

3. `git diff`: This command shows the differences between the changes made in the working directory and the last committed version, including local changes that have not been committed yet.

4. `git reset`: This command can be used to undo local changes and unstage them. It can also be used to revert local commits, but this should be done with caution, as it can potentially cause data loss.

Overall, local commits are important in the Git workflow as they enable developers to experiment with changes and track their progress before making them available to collaborators through remote commits. 

## tldr 
 
> Show local commits that haven't been pushed to origin. Any additional arguments will be passed directly to `git log`.
> Part of `git-extras.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-local-commits>.

- Show commits that haven't been pushed:

`git local-commits`
