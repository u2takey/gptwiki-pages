# dust 
## chatgpt 
As an AI language model, I cannot execute terminal commands nor operate applications/programs directly on my system. 
However, I can provide a brief description of the command 'dust' which is used in some Linux distributions.

The 'dust' command is generally used to display disk usage statistics in a visually appealing way. It can be used to show which files or directories are consuming the most amount of space on your system. Its output is displayed in a tabular format where each row represents a file or directory and the columns highlight the size, percentage of disk space used, and the associated file or directory name. The command recursively scans the given directory, meaning it calculates the disk usage of a directory and all of its sub-directories.

Overall, using the 'dust' command is a quick and easy way to analyze your system's disk usage and find ways to free up space. 

## tldr 
 
> Dust gives an instant overview of which directories are using disk space.
> More information: <https://github.com/bootandy/dust>.

- Display information for the current directory:

`dust`

- Display information for a space-separated list of directories:

`dust {{path/to/directory1}} {{path/to/directory2}}`

- Display 30 directories (defaults to 21):

`dust --number-of-lines {{30}}`

- Display information for the current directory, up to 3 levels deep:

`dust --depth {{3}}`

- Display the biggest directories at the top in descending order:

`dust --reverse`

- Ignore all files and directories with a specific name:

`dust --ignore-directory {{file_or_directory_name}}`

- Do not display percent bars and percentages:

`dust --no-percent-bars`
