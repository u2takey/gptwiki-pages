# dirname 
## chatgpt 
The "dirname" command is used to extract the directory name from a given path or file name. 

For example, if the path is '/home/user/documents/file.txt', the "dirname" command will extract '/home/user/documents' as the directory name.

The basic syntax of the "dirname" command is as follows:

dirname [path/file name]

Some common options that can be used with this command are:

- -z or --zero: Output null character after each directory name.
- -v or --verbose: Display the directory name along with the path.
- -h or --help: Display help information about the command.

Overall, the "dirname" command can be very useful for script writing and automation tasks where you need to extract directory names from paths or file names. 

## tldr 
 
> Calculates the parent directory of a given file or directory path.
> More information: <https://www.gnu.org/software/coreutils/dirname>.

- Calculate the parent directory of a given path:

`dirname {{path/to/file_or_directory}}`

- Calculate the parent directory of multiple paths:

`dirname {{path/to/file_a}} {{path/to/directory_b}}`

- Delimit output with a NUL character instead of a newline (useful when combining with `xargs`):

`dirname --zero {{path/to/directory_a}} {{path/to/file_b}}`
