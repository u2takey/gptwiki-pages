# git effort 
## chatgpt 
As an AI language model, I don't have access to any contextual information to exactly know what you mean by "git effort" command. However, assuming that you're referring to a command that displays the amount of work done by each author in a repository, here's a possible explanation:

Git doesn't have a built-in command called "git effort". However, there are third-party tools and git aliases that allow you to measure and visualize the contribution of each contributor. Here are some examples:

1. Git Extras: It's a collection of useful git commands that extends the built-in functionalities. One of the commands is "git effort", which shows the number of commits per author, the lines added and removed, and the percentage of total work. You can install Git Extras by following the instructions on their website.

2. Git Stats: It's a simple tool that generates a report of your git repository contribution. It shows the number of commits, lines added and removed, and the percentage of total work for each author. You can install Git Stats by following the instructions on their GitHub repository.

3. Git Alias: You can create a custom git alias that runs a script to calculate the contribution of each author. For example, you can create an alias called "git effort" that runs the following command:

`git log --pretty='%aN' | sort | uniq -c | sort -rn`

This command lists all the authors who contributed to the repository, sorted by the number of commits. Each line shows the number of commits and the author's name. You can modify the command to add more details such as the lines added and removed.

Overall, these tools and techniques help you understand the level of contribution of each author in a git repository, which can be useful for project management and team collaboration. 

## tldr 
 
> Display how much activity a file has had, showing commits per file and "active days" i.e. total number of days that contributed to the file.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-effort>.

- Display each file in the repository, showing commits and active days:

`git effort`

- Display files modified by a specific number of commits or more, showing commits and active days:

`git effort --above {{5}}`

- Display files modified by a specific author, showing commits and active days:

`git effort -- --author="{{username}}"`

- Display files modified since a specific time/date, showing commits and active days:

`git effort -- --since="{{last month}}"`

- Display only the specified files or directories, showing commits and active days:

`git effort {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Display all files in a specific directory, showing commits and active days:

`git effort {{path/to/directory/*}}`
