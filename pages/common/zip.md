# zip 
## chatgpt 
The "zip" command is a utility used for compressing archive files. It is a command-line tool that allows a user to create, modify, and extract compressed archives of files and folders.

The basic syntax of the command is:

zip [options] zipfile file1 [file2 ...]

Where:

- [options]: Represents the various options that can be used with the command. These options may include flags for compressing files, excluding certain files, and setting the compression level.
- zipfile: Specifies the name of the output archive file. This file will be created by the zip command.
- file1 [file2…]: Represents the names of the files or directories that are to be added to the output archive file.

Some of the commonly used options with the zip command are:

- -r: Specifies that the archive should be recursively compressed, i.e., it will include all the files and directories within any subdirectories.
- -q: Enables the "quiet" mode. This option suppresses any log messages or errors that may be output by the command.
- -9: Sets the maximum level of compression. This option is used to get the smallest possible archive size, but at the cost of longer compression time.
- -u: Updates an existing archive by adding new or modified files to it.

Overall, the zip command is a powerful tool for compressing files and directories, and can be used in conjunction with other commands or scripts to automate compression tasks. 

## tldr 
 
> Package and compress (archive) files into zip file.
> See also: `unzip`.
> More information: <https://manned.org/zip>.

- Add files/directories to a specific archive ([r]ecursively):

`zip -r {{path/to/compressed.zip}} {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Remove files/directories from a specific archive ([d]elete):

`zip -d {{path/to/compressed.zip}} {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Archive files/directories e[x]cluding specified ones:

`zip -r {{path/to/compressed.zip}} {{path/to/file_or_directory1 path/to/file_or_directory2 ...}} -x {{path/to/excluded_files_or_directories}}`

- Archive files/directories with a specific compression level (`0` - the lowest, `9` - the highest):

`zip -r -{{0-9}} {{path/to/compressed.zip}} {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Create an [e]ncrypted archive with a specific password:

`zip -r -e {{path/to/compressed.zip}} {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Archive files/directories to a multi-part [s]plit zip file (e.g. 3 GB parts):

`zip -r -s {{3g}} {{path/to/compressed.zip}} {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Print a specific archive contents:

`zip -sf {{path/to/compressed.zip}}`
