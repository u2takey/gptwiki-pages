# git diff 
## chatgpt 
The `git diff` command is used to compare the changes between two states of a repository. It can be used to compare branches, commits, or individual files. 

When used with no arguments, `git diff` will display the changes between the working directory and the latest commit. If a file name is specified as an argument, the command will display the changes for that particular file. 

The output of `git diff` shows lines that have been added or deleted, as well as any modifications to existing lines. Lines that have been added are shown in green, while lines that have been deleted are shown in red. The command also displays a summary of the differences at the end of the output, indicating the number of lines that have been added and deleted.

`git diff` can also be used with various options, such as `--color-words` to display the differences word-by-word instead of line-by-line, or `-U <num>` to specify the number of lines of context to display around the changes. 

Overall, `git diff` is a powerful tool for inspecting the changes to a repository and can be used to spot errors, debug issues or track changes over time. 

## tldr 
 
> Show changes to tracked files.
> More information: <https://git-scm.com/docs/git-diff>.

- Show unstaged, uncommitted changes:

`git diff`

- Show all uncommitted changes (including staged ones):

`git diff HEAD`

- Show only staged (added, but not yet committed) changes:

`git diff --staged`

- Show changes from all commits since a given date/time (a date expression, e.g. "1 week 2 days" or an ISO date):

`git diff 'HEAD@{3 months|weeks|days|hours|seconds ago}'`

- Show only names of changed files since a given commit:

`git diff --name-only {{commit}}`

- Output a summary of file creations, renames and mode changes since a given commit:

`git diff --summary {{commit}}`

- Compare a single file between two branches or commits:

`git diff {{branch_1}}..{{branch_2}} [--] {{path/to/file}}`

- Compare different files from the current branch to other branch:

`git diff {{branch}}:{{path/to/file2}} {{path/to/file}}`
