# rga 
## chatgpt 
The command "rga" is a search tool that allows users to search for specific text patterns within files located within a specified directory or recursively within subdirectories. "rga" stands for "ripgrep-all" which is its full name.

The command has the following syntax: 

``` rga [options] PATTERN [PATH...] ```

where "PATTERN" is the text string to search for and "PATH" is the location of the files to search in. 

Options that can be included with the command include:
- `-i` : ignore case when searching
- `-w` : match whole words only
- `-v` : invert the search and show lines that do not match the pattern
- `--hidden` : search hidden files and directories as well
- `-g` : use glob pattern to search for files instead of regular expressions
- `--files-with-matches` : show only the names of the files that contain matches
- `--count` : output the count of matches instead of the matching lines

Overall, "rga" is a powerful tool that can search through large files and directories quickly and efficiently, making it a useful asset for programmers and developers who need to search through code or log files. 

## tldr 
 
> Ripgrep wrapper with rich file type searching capabilities.
> More information: <https://github.com/phiresky/ripgrep-all>.

- Search recursively for a pattern in all files in the current directory:

`rga {{regular_expression}}`

- List available adapters:

`rga --rga-list-adapters`

- Change which adapters to use (e.g. ffmpeg, pandoc, poppler etc.):

`rga --rga-adapters={{adapter1,adapter2}} {{regular_expression}}`

- Search for a pattern using the mime type instead of the file extension (slower):

`rga --rga-accurate {{regular_expression}}`

- Display detailed help:

`rga --help`
