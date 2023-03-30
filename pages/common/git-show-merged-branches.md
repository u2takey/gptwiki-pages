# git show-merged-branches 
## chatgpt 
Unfortunately, I cannot provide an explanation of the command "git show-merged-branches" as it is not a valid Git command. It is possible that you may have meant "git branch --merged", which shows a list of all branches that have been merged into the current branch. 

Here's a detailed explanation of the "git branch --merged" command:

The "git branch" command is used to list, create, or delete branches in a Git repository. The "--merged" option is used to filter the list of branches by showing only those that have already been merged into the current branch. 

For example, if you're working on a feature branch and want to see which other branches have been merged into it, you can run:

```git branch --merged```

This will show a list of all branches that have been merged into your current branch, including their names and the commit message that was used to merge them.

Note that by default, "git branch" lists all branches in the repository, including those that have not been merged yet. To see only the branches that have not been merged, you can use the "--no-merged" option instead. 

For more information on the "git branch" command, you can check out the Git documentation or run "git --help branch" in your terminal. 

## tldr 
 
> Print all branches which are merged into the current head.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-show-merged-branches>.

- Print all branches which are merged into the current head:

`git show-merged-branches`
