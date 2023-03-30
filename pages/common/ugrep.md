# ugrep 
## chatgpt 
The ugrep command is a Unix/Linux command line tool that allows users to search for text patterns in files and directories. It is a more advanced version of the traditional grep command, with improved features and performance.

Here are some of the key features and options of the ugrep command:

1. Syntax: The basic syntax of the ugrep command is as follows:

   ```
   ugrep [options] pattern [files/directories]
   ```

2. Patterns: The ugrep command allows users to search for patterns in several formats, such as regular expressions, glob patterns, and even fuzzy matching.

3. Options: The ugrep command comes with several options to customize the search behavior, including:

   - Case sensitivity options: `-i` (case-insensitive), `-s` (case-sensitive).
   - Output options: `-H` (show file names), `-C` (show context), `-n` (show line numbers).
   - File filtering options: `-r` (search recursively), `-l` (show file names only), `-L` (show files that do not match).
   - Pattern options: `-w` (match whole words only), `-m` (limit the number of matches), `-f` (search for patterns from a file).
   
4. Examples: Here are some examples of using the ugrep command:

   - Search for a pattern in a file:
   
     ```
     ugrep pattern file.txt
     ```
   
   - Search for a pattern in a directory recursively:
   
     ```
     ugrep -r pattern dir/
     ```
   
   - Search for a pattern case-insensitively and show context:
   
     ```
     ugrep -i -C 3 pattern file.txt
     ```
   
   - Search for a pattern using a regular expression:
   
     ```
     ugrep '[0-9]{3}-[0-9]{2}-[0-9]{4}' file.txt
     ```
   
Overall, the ugrep command is a powerful tool for searching for text patterns in Unix/Linux systems, with many features and options to customize the search behavior. 

## tldr 
 
> Ultra fast search tool with query TUI.
> More information: <https://github.com/Genivia/ugrep>.

- Start a query TUI to search files in the current directory recursively (CTRL-Z for help):

`ugrep --query`

- Search the current directory recursively for files containing a regex search pattern:

`ugrep "{{search_pattern}}"`

- Search in a specific file or in all files in a specific directory, showing line numbers of matches:

`ugrep --line-number "{{search_pattern}}" {{path/to/file_or_directory}}`

- Search in all files in the current directory recursively and print the name of each matching file:

`ugrep --files-with-matches "{{search_pattern}}"`

- Fuzzy search files with up to 3 extra, missing or mismatching characters in the pattern:

`ugrep --fuzzy={{3}} "{{search_pattern}}"`

- Also search compressed files, `zip` and `tar` archives recursively:

`ugrep --decompress "{{search_pattern}}"`

- Search only files whose filenames match a specific glob pattern:

`ugrep --glob="{{glob_pattern}}" "{{search_pattern}}"`

- Search only C++ source files (use `--file-type=list` to list all file types):

`ugrep --file-type=cpp "{{search_pattern}}"`
