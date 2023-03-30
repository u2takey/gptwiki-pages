# hg add 
## chatgpt 
The "hg add" command is a command used in the Mercurial version control system. 

When files are added to a Mercurial repository, they are initially untracked. This means that Mercurial will not keep track of any changes made to them. In order to start tracking these files, the "hg add" command is used.

This command tells Mercurial to start tracking the specified files. This means that any changes made to these files will be recorded and can be reverted back to at any time in the future.

To use the "hg add" command, specific file names or directory names must be provided. The command can be used with wildcards and other arguments to specify which files/directories to add.

Once files have been added, they must be committed to the repository using the "hg commit" command in order to save the changes. 

## tldr 
 
> Adds specified files to the staging area for the next commit in Mercurial.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#add>.

- Add files or directories to the staging area:

`hg add {{path/to/file}}`

- Add all unstaged files matching a specified pattern:

`hg add --include {{pattern}}`

- Add all unstaged files, excluding those that match a specified pattern:

`hg add --exclude {{pattern}}`

- Recursively add sub-repositories:

`hg add --subrepos`

- Perform a test-run without performing any actions:

`hg add --dry-run`
