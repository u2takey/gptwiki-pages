# ripgrep 
## chatgpt 
Ripgrep is a command line tool used to search for a string or regular expression pattern in files within a specified directory hierarchy. It is a faster alternative to the traditional grep command, and can search through large directories and files much quicker.

Syntax: `rg [OPTIONS] PATTERN [PATHS...]`

Where:

- `[OPTIONS]`: specify optional search parameters like `-i` to ignore case distinctions or `-v` to print lines not matching the pattern.
- `PATTERN`: the regular expression or string to search for.
- `[PATHS...]`: the file paths where the search will be conducted.

Ripgrep searches through files recursively by default, so it will search through all files in the specified directories and subdirectories. It also automatically ignores hidden files and directories, binary files, and files listed in `.gitignore`.

Additionally, ripgrep supports many features like recursive search, case-insensitive search, displaying line numbers and file names, ignoring certain directories or files, and more. 

## tldr 
 
> `ripgrep` is the common name for the command `rg`.

- View documentation for the original command:

`tldr rg`
