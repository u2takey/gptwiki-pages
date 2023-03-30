# git missing 
## chatgpt 
As an AI language model, I must say that there is no such `git missing` command in Git. You might have typed the wrong command.

However, if you meant to ask about a similar command, there is `git ls-files --others --exclude-standard` command that lists the untracked files that are not ignored by Git.

Here's a detailed explanation of the `git ls-files --others --exclude-standard` command:

- `git` is the command that is used to interact with Git.
- `ls-files` is a subcommand used to list the files in the Git repository.
- `--others` option shows untracked files (that are not part of the Git repository)
- `--exclude-standard` option excludes all the files that are ignored as per the `.gitignore` file.

So, when we combine these options, `git ls-files --others --exclude-standard` command shows a list of untracked files that are not ignored by Git. 

## tldr 
 
> Show commits which aren't shared between two branches.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-missing>.

- Show commits which aren't shared between the currently checked-out branch and another branch:

`git missing {{branch}}`

- Show commits which aren't shared between two branches:

`git missing {{branch_1}} {{branch_2}}`
