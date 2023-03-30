# git clean 
## chatgpt 
The `git clean` command is used to remove untracked files from the current working directory. These untracked files might be any file or directory that is not being tracked by Git repository, which includes new files that have not been added to the repository, files that have been locally created, edited, or deleted, and any other files or directories that are not included in the repository. 

Here are the basic parameters for the `git clean` command:

`-n` or `--dry-run`: This flag displays the list of untracked files that will be removed without actually deleting them.

`-f` or `--force`: This flag performs the actual removal of untracked files.

`-d` or `--directory`: This flag tells git to remove directories as well.

There are also some other options of `git clean` command which include:

`-i` or `--interactive`: This flag lets you interactively review the files before deletion.

`-e` or `--exclude`: This flag lets you exclude certain files from being removed.

`-x` or `--force`: This flag removes both tracked and untracked files.

Overall, `git clean` is a very useful command for cleaning up your working directory and can be used to free up space, remove unnecessary files and declutter your files before committing. 

## tldr 
 
> Remove untracked files from the working tree.
> More information: <https://git-scm.com/docs/git-clean>.

- Delete files that are not tracked by Git:

`git clean`

- Interactively delete files that are not tracked by Git:

`git clean -i`

- Show what files would be deleted without actually deleting them:

`git clean --dry-run`

- Forcefully delete files that are not tracked by Git:

`git clean -f`

- Forcefully delete directories that are not tracked by Git:

`git clean -fd`

- Delete untracked files, including ignored files in `.gitignore` and `.git/info/exclude`:

`git clean -x`
