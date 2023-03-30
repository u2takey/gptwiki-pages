# rar 
## chatgpt 
The "rar" command is an executable program used for compression, archiving, and extraction of files in the RAR format, developed by RARLAB. 

The command has several options that allow users to customize the compression and archiving process according to their requirements. Some of the common options include:

- "a": This option is used to add files to an existing archive. For example, "rar a archive.rar file1.txt file2.png" creates or updates the "archive.rar" file to include the specified files. 

- "x": This option is used to extract files from an archive. For example, "rar x archive.rar" extracts all files from the "archive.rar" file in the current directory. 

- "c": This option is used to create a new archive. For example, "rar c new-archive.rar file1.txt file2.png" creates a new archive "new-archive.rar" with the specified files. 

- "t": This option is used to test the integrity of an archive. For example, "rar t archive.rar" tests the integrity of the "archive.rar" file and reports any errors. 

- "v": This option is used for verbose output, which displays detailed information about the compression or extraction process. 

Some other options include specifying the compression level (-m), password protection (-p), file exclusion (-x), and more. The "rar" command is generally used in a terminal or command prompt window in various operating systems, such as Windows, Linux, and macOS. 

## tldr 
 
> The RAR archiver. Supports multi-volume archives that can be optionally self-extracting.
> More information: <https://manned.org/rar>.

- Archive 1 or more files:

`rar a {{path/to/archive_name.rar}} {{path/to/file1}} {{path/to/file2}} {{path/to/file3}}`

- Archive a directory:

`rar a {{path/to/archive_name.rar}} {{path/to/directory}}`

- Split the archive into parts of equal size (50M):

`rar a -v{{50M}} -R {{path/to/archive_name.rar}} {{path/to/file_or_directory}}`

- Password protect the resulting archive:

`rar a -p{{password}} {{path/to/archive_name.rar}} {{path/to/file_or_directory}}`

- Encrypt file data and headers with password:

`rar a -hp{{password}} {{path/to/archive_name.rar}} {{path/to/file_or_directory}}`

- Use a specific compression level (0-5):

`rar a -m{{compression_level}} {{path/to/archive_name.rar}} {{path/to/file_or_directory}}`
