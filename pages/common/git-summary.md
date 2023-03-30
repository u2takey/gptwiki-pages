# git summary 
## chatgpt 
As an AI language model, I can explain the git command but not the "git summary" command; as there is no "git summary" command in Git documentation. But I can explain the "git log --summary" command, which provides a summary of the changes for each commit. 

The "git log --summary" command is used to display a detailed summary of each commit, including the commit hash, author, date, commit message, and a summary of the changes made in the commit. The summary includes the number of files changed, the number of lines added and removed, and the file names. 

When you run this command, Git generates the commit history for the current branch, starting from the most recent commit and working backwards through history. All the changes in each commit are summarized, providing a high-level overview of the changes made in the project over time. 

It’s a useful command for reviewing and understanding changes made in a project, as it allows you to see at a glance how the project has evolved and how changes have been implemented. Additionally, you can use various options and filters with the "git log --summary" command to refine the output and narrow down the information you need. 

## tldr 
 
> Display information about a Git repository.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-summary>.

- Display data about a Git repository:

`git summary`

- Display data about a Git repository since a commit-ish:

`git summary {{commit|branch_name|tag_name}}`

- Display data about a Git repository, merging committers using different emails into 1 statistic for each author:

`git summary --dedup-by-email`

- Display data about a Git repository, showing the number of lines modified by each contributor:

`git summary --line`
