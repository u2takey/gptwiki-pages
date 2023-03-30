# diskonaut 
## chatgpt 
Diskonaut is a command-line interface (CLI) utility that helps in visualizing disk usage on Linux, Windows or macOS systems. It scans the entire file system and shows an interactive, colored tree map that represents the size of all directories and files. This tool can be used to:

1. Understand how and where disk space is being used.
2. Identify large files and directories that may be taking up unnecessary space.
3. Delete or move unwanted or redundant files and directories to free up space.

Some of the basic commands and flags used in Diskonaut are:

1. `diskonaut`: This command runs the tool and displays the tree map in the terminal.
2. `diskonaut -h` or `diskonaut --help`: This displays the help menu with all the available commands and flags.
3. `diskonaut -d <directory>` or `diskonaut --directory <directory>`: This runs the tool on a specific directory.
4. `diskonaut -x <extension>` or `diskonaut --exclude <extension>`: This excludes the file types with the specified extension from the output.
5. `diskonaut -t <size>` or `diskonaut --size-threshold <size>`: This sets the size threshold for displaying files and directories in the tree map.
6. `diskonaut -s` or `diskonaut --sort-by-size`: This sorts the files and directories in the tree map by size.

Overall, Diskonaut is a useful tool for identifying and managing disk space usage on a system. 

## tldr 
 
> Terminal disk space navigator, written in Rust.
> More information: <https://github.com/imsnif/diskonaut>.

- Start diskonaut in the current directory:

`diskonaut`

- Start diskonaut in a specific directory:

`diskonaut {{path/to/directory}}`

- Show file sizes rather than their block usage on the disk:

`diskonaut --apparent-size {{path/to/directory}}`

- Disable deletion confirmation:

`diskonaut --disable-delete-confirmation`
