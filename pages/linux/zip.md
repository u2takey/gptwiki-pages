# zip 
## chatgpt 
The `zip` command is used to create, add, extract and view compressed archives in the ZIP file format.

Here are the basic syntax and options of the `zip` command:

```
zip [options] archive_name file1 [file2 ...]
```

Options:
- `-r`: Recursively compress an entire directory and its contents.
- `-q`: Quiet mode, suppresses output except for error messages.
- `-d`: Delete files from the archive.
- `-u`: Update an existing archive with new files.
- `-v`: Verbose mode, displays the compression progress and list of files added to the archive.

Example Usage:

1. Create a new archive:
```
zip archive_name.zip file1.txt file2.txt
```
This command creates a new ZIP archive called `archive_name.zip` and adds two files `file1.txt` and `file2.txt` to it.

2. Extract files from an archive:
```
unzip archive_name.zip
```
This command extracts all the files in the `archive_name.zip` archive to the current directory.

3. Add a directory and its contents to an archive:
```
zip -r new_archive.zip directory_name
```
This command compresses the entire `directory_name` folder and its contents into a new ZIP archive called `new_archive.zip`.

4. Delete a file from an archive:
```
zip -d archive_name.zip file1.txt
```
This command deletes `file1.txt` from the `archive_name.zip` archive.

5. Update an existing archive with new files:
```
zip -u archive_name.zip file3.txt
```
This command adds `file3.txt` to the existing `archive_name.zip` archive if it doesn't exist or updates it if it does. 

## tldr 
 
> Package and compress (archive) files into zip file.
> See also: `unzip`.
> More information: <https://manned.org/zip>.

- Add files/directories to a specific archive:

`zip -r {{path/to/compressed.zip}} {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Remove files/directories from a specific archive:

`zip --delete {{path/to/compressed.zip}} {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Archive files/directories e[x]cluding specified ones:

`zip {{path/to/compressed.zip}} {{path/to/file_or_directory1 path/to/file_or_directory2 ...}} --exclude {{path/to/excluded_files_or_directories}}`

- Archive files/directories with a specific compression level (`0` - the lowest, `9` - the highest):

`zip -r -{{0-9}} {{path/to/compressed.zip}} {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Create an encrypted archive with a specific password:

`zip -r --encrypt {{path/to/compressed.zip}} {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Archive files/directories to a multi-part [s]plit zip file (e.g. 3 GB parts):

`zip -r -s {{3g}} {{path/to/compressed.zip}} {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Print a specific archive contents:

`zip -sf {{path/to/compressed.zip}}`
