# find 
## chatgpt 
The "find" command in Linux is used to search for files and directories in the file system hierarchy. It is a powerful tool that allows the user to search for files and directories using various search criteria such as name, size, type, modification date, permissions, and more. 

The basic syntax of the "find" command is as follows:

find [path] [expression]

Where "path" is the location you want to search, and "expression" is the criteria you want to use to find files and directories. 

Some common examples of using the "find" command are:

1. Finding a file by name:

To find a file called "example.txt" in the current directory and its subdirectories, the command would be:

find . -name example.txt

The "." indicates the current directory.

2. Finding files by type:

To find all files with the extension ".txt" in the current directory and its subdirectories, the command would be:

find . -type f -name "*.txt"

The "-type f" option specifies that we want to search for files only, not directories.

3. Finding directories with certain permissions:

To find all directories in the current directory and its subdirectories that have read, write, and execute permissions for the owner, the command would be:

find . -type d -perm 700

The "-perm 700" option specifies that we want to find directories with permission "rwx------" (i.e., only the owner can read, write, and execute).

There are many other ways to use the "find" command to search for files and directories. The command is highly versatile and can be customized to suit specific search criteria. 

## tldr 
 
> Find files or directories under the given directory tree, recursively.
> More information: <https://manned.org/find>.

- Find files by extension:

`find {{root_path}} -name '{{*.ext}}'`

- Find files matching multiple path/name patterns:

`find {{root_path}} -path '{{**/path/**/*.ext}}' -or -name '{{*pattern*}}'`

- Find directories matching a given name, in case-insensitive mode:

`find {{root_path}} -type d -iname '{{*lib*}}'`

- Find files matching a given pattern, excluding specific paths:

`find {{root_path}} -name '{{*.py}}' -not -path '{{*/site-packages/*}}'`

- Find files matching a given size range, limiting the recursive depth to "1"::

`find {{root_path}} -maxdepth 1 -size {{+500k}} -size {{-10M}}`

- Run a command for each file (use `{}` within the command to access the filename):

`find {{root_path}} -name '{{*.ext}}' -exec {{wc -l {} }}\;`

- Find files modified in the last 7 days:

`find {{root_path}} -daystart -mtime -{{7}}`

- Find empty (0 byte) files and delete them:

`find {{root_path}} -type {{f}} -empty -delete`
