# hg update 
## chatgpt 
The "hg update" command is a command used in the Mercurial version control system. It is used to update the current working directory to a specific revision or branch in the repository.

When you run the "hg update" command, Mercurial will update your current working directory and the files within it to match the specified revision or branch. This means that any changes you have made to your local files that are not committed will be lost unless you have saved them elsewhere.

The "hg update" command also has several options that can be used to control how the update process is handled. These options include "-C" to discard any local changes made to the files, "-r" to specify a revision number or branch, "-b" to specify a branch to update to, and "-clean" to remove any untracked files or directories.

Overall, the "hg update" command is an important command for managing your repository and ensuring that your local copy is synced up with the latest changes in the project. 

## tldr 
 
> Update the working directory to a specified changeset.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#update>.

- Update to the tip of the current branch:

`hg update`

- Update to the specified revision:

`hg update --rev {{revision}}`

- Update and discard uncommitted changes:

`hg update --clean`

- Update to the last commit matching a specified date:

`hg update --date {{dd-mm-yyyy}}`
