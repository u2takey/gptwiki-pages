# exa 
## chatgpt 
The "exa" command is a modern replacement for the traditional "ls" command that displays files and directories in a terminal. It is a third-party, open-source tool that provides additional features and customization options compared to the traditional "ls" command. Some of the features of the "exa" command include:

1. Colorized output: The "exa" command shows different colors for different types of files and directories, making it easier to identify them at a glance.

2. Human-readable file sizes: The file sizes are displayed in readable formats like KB, MB or GB instead of bytes.

3. Git integration: If the current directory is a Git repository, "exa" shows the Git status of the files.

4. Support for Unicode characters: The "exa" command correctly displays Unicode characters in the file or directory names.

5. Multiple output formats: "exa" can display the output in different formats like tree view, long format or short format.

6. Sorting: "exa" allows sorting of files and directories based on different criteria like name, size or modification time.

The "exa" command can be used with various options and flags to customize the output. For example, using "exa -l" will display the files and directories in the long format, while "exa -h" displays the file sizes in human-readable format. Overall, the "exa" command is a powerful replacement for the traditional "ls" command that offers more features and customization options to users. 

## tldr 
 
> A modern replacement for `ls` (List directory contents).
> More information: <https://the.exa.website>.

- List files one per line:

`exa --oneline`

- List all files, including hidden files:

`exa --all`

- Long format list (permissions, ownership, size and modification date) of all files:

`exa --long --all`

- List files with the largest at the top:

`exa --reverse --sort={{size}}`

- Display a tree of files, three levels deep:

`exa --long --tree --level={{3}}`

- List files sorted by modification date (oldest first):

`exa --long --sort={{modified}}`

- List files with their headers, icons, and Git statuses:

`exa --long --header --icons --git`

- Don't list files mentioned in `.gitignore`:

`exa --git-ignore`
