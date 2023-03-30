# git delete-branch 
## chatgpt 
The command "git delete-branch" is not a built-in Git command, so it is not an actual Git command. 

However, to remove a branch in Git, the correct syntax is:

```
git branch -d <branch_name>
```

This command will delete the specified branch from the local repository. If the branch has not been merged, you can use the "-D" option instead to force the deletion.

```
git branch -D <branch_name>
```

Before deleting a branch, ensure that you have committed all your changes and that the branch has been merged, or that you have saved any necessary changes from the branch before deleting it. 

## tldr 
 
> Delete local and remote Git branches.
> Part of `git-extras`. If deleting the checked out branch, only the remote branch will be deleted.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-delete-branch>.

- Delete a local and remote Git branch:

`git delete-branch {{branch_name}}`

- Delete multiple local and remote Git branches:

`git delete-branch {{branch_name1 branch_name2 ...}}`
