# git rename-branch 
## chatgpt 
The `git rename-branch` command is used to rename a branch in a Git repository. The syntax for the command is as follows:

```
git rename-branch <old-branch-name> <new-branch-name>
```

The command renames an existing branch with the given `<old-branch-name>` to `<new-branch-name>`. 

Here are some key points to keep in mind when using `git rename-branch`:

1. The command changes the name of the branch only within the local repository. If the branch has already been pushed to a remote repository, the remote branch name will remain unchanged until you explicitly push the renamed branch to the remote repository.

2. Before renaming a branch, make sure that you are not currently checked out to that branch. You can switch to another branch by running `git checkout <branch-name>` command.

3. Renaming a branch does not affect its commit history. All the commits associated with the old branch name are still accessible from the new branch name.

4. If you have any local branches that track the renamed branch, you need to update their name as well. You can use the `git branch -m <old-branch-name> <new-branch-name>` command to do so.

Overall, `git rename-branch` is a useful command for renaming branches in your local repository. It can help you keep your branch names consistent and make it easier to manage your codebase. 

## tldr 
 
> Rename a Git branch.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-rename-branch>.

- Rename the branch you are currently on:

`git rename-branch {{new_branch_name}}`

- Rename a specific branch:

`git rename-branch {{old_branch_name}} {{new_branch_name}}`
