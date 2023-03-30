# git delete-merged-branches 
## chatgpt 
The command "git delete-merged-branches" is not a default command in Git. However, it might refer to a custom script or alias that is created to delete branches that have been merged into the current branch.

Here's how the command/script would generally work:

1. It first checks the current branch (usually the main branch, such as master or main).

2. It then uses the "git branch --merged" command to get the list of branches that have been merged into the current branch.

3. It might then prompt the user to confirm the branch deletions, as a safety measure.

4. Finally, for each of the merged branches, it uses the "git branch -d" command to delete the branch.

This command can be useful to clean up old and irrelevant branches that are no longer needed, simplifying the branch navigation and cleaning up the repository history. However, it's important to exercise caution when deleting branches, as they might contain valuable information and history that cannot be easily retrieved once deleted. 

## tldr 
 
> Delete branches that are listed in `git branch --merged` excluding master.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-delete-merged-branches>.

- Delete merged branches:

`git delete-merged-branches`
