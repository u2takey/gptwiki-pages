# hg status 
## chatgpt 
The "hg status" command is a command used in the Mercurial version control system. 

This command is used to show the current status of the repository. It displays a list of the files in the repository along with their current status, such as whether they have been modified, added or deleted. 

Here is a breakdown of the different status indicators:

- `M` - Modified: The file has been modified since its last commit. 
- `A` - Added: The file has been newly added to the repository and has not yet been committed. 
- `R` - Removed: The file has been removed from the repository since its last commit. 
- `C` - Clean: The file is unchanged and matches the most recent commit. 
- `!` - Missing: The file is missing from the repository. 
- `?` - Unknown: The file is present in the working directory but not tracked by Mercurial. 

By default, "hg status" only shows files with changes. You can use the "hg status -A" command to show all files, including those that are unchanged. 

The "hg status" command is often used as a quick way to check the status of the working directory before committing changes. If you see any modified or added files, you can use the "hg add" command to add them to the staging area, and then use "hg commit" to commit the changes to the repository. 

## tldr 
 
> Show files that have changed in the working directory.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#status>.

- Display the status of changed files:

`hg status`

- Display only modified files:

`hg status --modified`

- Display only added files:

`hg status --added`

- Display only removed files:

`hg status --removed`

- Display only deleted (but tracked) files:

`hg status --deleted`

- Display changes in the working directory compared to a specified changeset:

`hg status --rev {{revision}}`

- Display only files matching a specified glob pattern:

`hg status --include {{pattern}}`

- Display files, excluding those that match a specified glob pattern:

`hg status --exclude {{pattern}}`
