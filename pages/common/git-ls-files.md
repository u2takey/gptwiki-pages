# git ls-files 
## chatgpt 
The `git ls-files` command lists all the files that are currently tracked by Git in the working directory and subdirectories. 

When you execute the `git ls-files` command, it will output a list of all files that are currently being tracked by Git on the current branch. This means that the command will show files that have been staged, committed, or are still in the working directory waiting to be committed.

Furthermore, you can specify options to modify the behavior of the `git ls-files` command. For example, you can use the `-s` option to display the object name and mode in addition to the file name. Or, you can use the `--eol` option to print the line endings for each file.

Overall, `git ls-files` is a useful command to review the status of your files in the Git repository and can be used in conjunction with other Git commands (such as `git status`, `git add`, and `git commit`) to manage and track changes to your codebase. 

## tldr 
 
> Show information about files in the index and the working tree.
> More information: <https://git-scm.com/docs/git-ls-files>.

- Show deleted files:

`git ls-files --deleted`

- Show modified and deleted files:

`git ls-files --modified`

- Show ignored and untracked files:

`git ls-files --others`

- Show untracked files, not ignored:

`git ls-files --others --exclude-standard`
