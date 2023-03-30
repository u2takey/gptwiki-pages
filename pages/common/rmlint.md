# rmlint 
## chatgpt 
rmlint is a command-line utility tool used for finding and removing duplicate, broken, and dead files from a file system. It is an open-source tool that is available on most Linux distributions and can be installed from the official repositories. 

Basically, the rmlint command searches a specified directory and its subdirectories to identify duplicate and dead files. The duplicate files are then grouped together and marked for removal while the dead files are removed automatically. 

Some of the features of rmlint include the ability to search for hard links, fuzzy matching, ignoring empty files, and support for user-specified regular expressions. 

It is important to note that the rmlint command can be destructive, and files deleted by the command cannot be recovered. Therefore, it is recommended to backup important files before running the command to avoid losing important data. 

## tldr 
 
> Identify duplicate files or directories, and other filesystem issues.
> More information: <https://rmlint.readthedocs.io/en/latest/rmlint.1.html>.

- Check a directory for duplicates, empty files, and other issues:

`rmlint {{path/to/directory}}`

- Delete duplicate files found by an execution of `rmlint`:

`./rmlint.sh`

- Find duplicate directory trees:

`rmlint --merge-directories {{path/to/directory}}`

- Mark files at lower path [d]epth as originals:

`rmlint --rank-by={{d}} {{path/to/directory}}`

- Mark files with shortest name [l]ength as originals:

`rmlint --rank-by={{l}} {{path/to/directory}}`

- Find only duplicates that have the same filename in addition to the same contents:

`rmlint --match-basename {{path/to/directory}}`

- Find all duplicates with the same extension:

`rmlint --match-extension {{path/to/directory}}`
