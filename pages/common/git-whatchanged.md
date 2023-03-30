# git whatchanged 
## chatgpt 
The "git whatchanged" command lists all the changes made to the repository in reverse chronological order. It displays each commit along with the author, date, and commit message. Additionally, it provides a list of all files modified by each commit, along with the specific lines added or removed from the file.

The output of "git whatchanged" can be useful for auditing changes to the repository, understanding the history of a particular file, or identifying potential bugs or issues introduced by recent changes. It can also be helpful for identifying who made certain changes to the repository and why they were made.

By default, "git whatchanged" displays the entire history of the repository. However, you can also provide a range of revisions to limit the output to a specific subset of the repository's history. For example, you can use the "--since" and "--until" options to limit the output to a specific timeframe, or you can specify a particular commit range using the standard "start..end" format. 

## tldr 
 
> Show what has changed with recent commits or files.
> See also `git log`.
> More information: <https://git-scm.com/docs/git-whatchanged>.

- Display logs and changes for recent commits:

`git whatchanged`

- Display logs and changes for recent commits within the specified time frame:

`git whatchanged --since="{{2 hours ago}}"`

- Display logs and changes for recent commits for specific files or directories:

`git whatchanged {{path/to/file_or_directory}}`
