# rdfind 
## chatgpt 
Rdfind is a command-line tool used for finding duplicate files and directories in a file system. It identifies files that have the same content and removes the duplicates, freeing up space on your system. Here is some information about the command:

Syntax:
```
$ rdfind [options] directory or file(s)
```

Options:
- `-dryrun` or `-n`: This option performs a dry run and does not delete any files.
- `-makehardlinks` or `-mkhard`: This option replaces duplicate files with hard links.
- `-makesymlinks` or `-mksymlinks`: This option replaces duplicate files with symbolic links.
- `-followsymlinks` or `-follow`: This option follows symbolic links to find duplicate files and directories.
- `-ignoreempty` or `-ie`: This option ignores empty files and directories when searching for duplicates.
- `-ignorelinks` or `-il`: This option ignores symbolic links when searching for duplicates.
- `-minsize` or `-m`: This option specifies the minimum size of the files to consider when searching for duplicates.
- `-fd` or `-filesonly`: This option searches for duplicates only in files, ignoring directories.
- `-rd` or `-dirsonly`: This option searches for duplicates only in directories, ignoring files.

Example:
```
$ rdfind -makehardlinks /home/user/Documents
```
This command searches for duplicate files in the "Documents" folder of the current user's home directory and replaces them with hard links. 

## tldr 
 
> Find files with duplicate content and get rid of them.
> More information: <https://rdfind.pauldreik.se>.

- Identify all duplicates in a given directory and output a summary:

`rdfind -dryrun true {{path/to/directory}}`

- Replace all duplicates with hardlinks:

`rdfind -makehardlinks true {{path/to/directory}}`

- Replace all duplicates with symlinks/soft links:

`rdfind -makesymlinks true {{path/to/directory}}`

- Delete all duplicates and do not ignore empty files:

`rdfind -deleteduplicates true -ignoreempty false {{path/to/directory}}`
