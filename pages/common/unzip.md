# unzip 
## chatgpt 
The `unzip` command is a UNIX utility used to extract the contents of an archive in the ZIP format. This command is used to extract individual files or directories from a zipped archive. 

The syntax for the `unzip` command is:
```
unzip [option] [zipfile] [file-to-extract]
```
where:
- `option`: A set of optional flags that modify the behavior of the `unzip` command.
- `zipfile`: The name of the ZIP archive file that you want to extract.
- `file-to-extract`: The name of the file(s) or directory(s) that you want to extract from the ZIP archive.

Some of the commonly used options with the `unzip` command are:

- `-l`: Used to list the contents of a ZIP archive without extracting them.
- `-o`: Used to overwrite any existing files without prompting for confirmation.
- `-d`: Used to specify the directory where the extracted files will be placed.

Example:
Suppose you have a file `example.zip` that contains two files named `file1.txt` and `file2.txt`. You want to extract `file1.txt` from the ZIP archive, and you want to store it in the directory `/home/user/documents`. In this case, you would use the following command:

```
unzip example.zip file1.txt -d /home/user/documents
```

This command will extract `file1.txt` from the `example.zip` file and save it in the directory `/home/user/documents`. 

## tldr 
 
> Extract files/directories from ZIP archives.
> See also: `zip`.
> More information: <https://manned.org/unzip>.

- Extract all files/directories from specific archives into the current directory:

`unzip {{path/to/archive1.zip path/to/archive2.zip ...}}`

- Extract files/directories from archives to a specific path:

`unzip {{path/to/archive1.zip path/to/archive2.zip ...}} -d {{path/to/output}}`

- Extract files/directories from archives to `stdout`:

`unzip -c {{path/to/archive1.zip path/to/archive2.zip ...}}`

- Extract the contents of the file(s) to `stdout` alongside the extracted file names:

`unzip -O {{gbk}} {{path/to/archive1.zip path/to/archive2.zip ...}}`

- List the contents of a specific archive without extracting them:

`unzip -l {{path/to/archive.zip}}`

- Extract a specific file from an archive:

`unzip -j {{path/to/archive.zip}} {{path/to/file_in_archive1 path/to/file_in_archive2 ...}}`
