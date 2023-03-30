# tree 
## chatgpt 
`tree` is a command-line utility in UNIX-like operating systems. The `tree` command displays the file or directory hierarchy in a tree-like format. It is used to visualize the structure of directories and sub-directories in a clear and organized way.

To use the `tree` command, simply open a terminal or a Linux shell and type `tree` followed by an initial directory path. 

For example, to view the directory structure of the current directory, enter:

```
tree
```

This will display a tree-like diagram of the current directory, showing all subdirectories, files, and their hierarchical relationship.

By default, the `tree` command displays the hierarchy in a simple text-based format. However, you can use various options to customize the output, such as coloring directories based on their type and displaying file size, permissions, and modification times.

Here are some commonly used options with `tree`:

- `-a` - Show hidden files.
- `-d` - Only show directories in the tree.
- `--filelimit n` - Limit the display of files per directory. n is the number of files to display.
- `--dirsfirst` - List the directories before the files.
- `-l` - Follow symbolic links.
- `-L level` - Set the maximum tree depth. level is an integer.

Overall, the `tree` command is a very useful tool for understanding the layout of a file system and is often used by system administrators to troubleshoot and manage directories and files. 

## tldr 
 
> Show the contents of the current directory as a tree.
> More information: <http://mama.indstate.edu/users/ice/tree/>.

- Print files and directories up to 'num' levels of depth (where 1 means the current directory):

`tree -L {{num}}`

- Print directories only:

`tree -d`

- Print hidden files too with colorization on:

`tree -a -C`

- Print the tree without indentation lines, showing the full path instead (use `-N` to not escape non-printable characters):

`tree -i -f`

- Print the size of each file and the cumulative size of each directory, in human-readable format:

`tree -s -h --du`

- Print files within the tree hierarchy, using a wildcard (glob) pattern, and pruning out directories that don't contain matching files:

`tree -P '{{*.txt}}' --prune`

- Print directories within the tree hierarchy, using the wildcard (glob) pattern, and pruning out directories that aren't ancestors of the wanted one:

`tree -P {{directory_name}} --matchdirs --prune`

- Print the tree ignoring the given directories:

`tree -I '{{directory_name1|directory_name2}}'`
