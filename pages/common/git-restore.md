# git restore 
## chatgpt 
Git restore is a command used to restore the state of a file or a branch in a Git repository. It is similar to the "revert" command, but instead of creating a new commit that undoes the changes made in a previous commit, it simply restores the file or branch to its previous state.

The git restore command is used to undo changes made to a file in the working directory or to restore a file to a previous state. The syntax of the git restore command is as follows:

git restore [options] [path]

The options for git restore command include:

--staged: This option is used to restore changes made to a file that has been added to the staging area.

--source: This option is used to restore a file to a specific commit, branch or tag.

--worktree: This option is used to restore a file to its original state in the working directory.

The path in the git restore command is the path to the file or directory being restored.

For example, to restore a file named "example.txt" to its original state in the working directory, the following command can be used:

git restore --worktree example.txt

Similarly, to restore a file that has been added to the staging area, the following command can be used:

git restore --staged example.txt

And to restore a file to a specific commit, branch or tag, the following command can be used:

git restore --source=branch-name example.txt 

## tldr 
 
> Restore working tree files. Requires Git version 2.23+.
> See also `git checkout` and `git reset`.
> More information: <https://git-scm.com/docs/git-restore>.

- Restore an unstaged file to the version of the current commit (HEAD):

`git restore {{path/to/file}}`

- Restore an unstaged file to the version of a specific commit:

`git restore --source {{commit}} {{path/to/file}}`

- Discard all unstaged changes to tracked files:

`git restore :/`

- Unstage a file:

`git restore --staged {{path/to/file}}`

- Unstage all files:

`git restore --staged :/`

- Discard all changes to files, both staged and unstaged:

`git restore --worktree --staged :/`

- Interactively select sections of files to restore:

`git restore --patch`
