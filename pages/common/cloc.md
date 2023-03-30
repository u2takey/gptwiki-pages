# cloc 
## chatgpt 
cloc is a command line tool used for counting lines of code in various programming languages within a project. The command "cloc" is used to run the tool and get the line count data. 

Here's how you can use cloc command:

1. Install cloc on your system first.
2. Navigate to the project directory that you want to count the lines of code.
3. Open the terminal or command prompt in the directory.
4. Type the command "cloc" and press enter.
5. You should see the output with a summary of the number of files, lines of code, and more information.

Options:
- --exclude-dir: Allows you to exclude certain directories from being included in the line count.
- --exclude-lang: Allows you to exclude certain programming languages from being included in the line count.
- --by-file: Allows you to display individual line count for each file in the project.
- --csv: Allows to output the result in CSV format.

Overall, cloc is a useful tool for developers to quickly get an estimate of how complex a codebase is and how long it may take to complete the project. 

## tldr 
 
> Count, and compute differences of, lines of source code and comments.
> More information: <https://github.com/AlDanial/cloc>.

- Count all the lines of code in a directory:

`cloc {{path/to/directory}}`

- Count all the lines of code in a directory, displaying a progress bar during the counting process:

`cloc --progress=1 {{path/to/directory}}`

- Compare 2 directory structures and count the differences between them:

`cloc --diff {{path/to/directory/one}} {{path/to/directory/two}}`

- Ignore files that are ignored by VCS, such as files specified in `.gitignore`:

`cloc --vcs git {{path/to/directory}}`

- Count all the lines of code in a directory, displaying the results for each file instead of each language:

`cloc --by-file {{path/to/directory}}`
