# git pr 
## chatgpt 
"git pr" is not a valid Git command. However, "git pull --rebase" and "git push" are two separate Git commands that are often used when working with remote repositories, specifically when contributing to open-source projects.

1. git pull --rebase:
This command is used to fetch the latest changes from a remote repository, and then apply those changes to the local repository, effectively updating the local branch. The --rebase option tells Git to apply the changes from the remote branch to the local branch as if they were made in a linear sequence, instead of creating a separate merge commit.

If there are conflicts between the changes made on the local branch and the changes from the remote branch, the command will pause the rebase process to allow the user to resolve the conflicts before continuing. This command is often used before making changes to a local branch and contributing those changes to a remote repository.

2. git push:
This command is used to upload local changes to a remote repository. Once the changes are pushed to the remote repository, other developers can access and make changes to them.

The command requires a branch name to specify which branch to push the changes to. If the branch doesn't exist on the remote repository, it will be created. If the branch already exists, the changes will be added to the existing branch.

In order to successfully push a branch, the user needs to have write access to the remote repository and the branch. The changes made on the local branch need to be committed before they can be pushed. 

## tldr 
 
> Check out GitHub pull requests locally.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-pr>.

- Check out a specific pull request:

`git pr {{pr_number}}`

- Check out a pull request from a specific remote:

`git pr {{pr_number}} {{remote}}`

- Check out a pull request from its URL:

`git pr {{url}}`

- Clean up old pull request branches:

`git pr clean`
