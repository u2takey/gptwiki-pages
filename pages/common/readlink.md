# readlink 
## chatgpt 
The `readlink` command is used in Linux and Unix systems to display the target of a symbolic link. A symbolic link is a special type of file that acts as a pointer to another file or directory.

The basic syntax of the `readlink` command is:

```
readlink [option] symbolic_link_name
```

Here, `symbolic_link_name` is the name or path of the symbolic link you want to view. 

Optionally, you can use the following options with the `readlink` command:

- `-f`: Displays the absolute path of the target file or directory.
- `-m`: Resolves the symbolic link to a canonicalized path.
- `-e`: Displays the absolute path of the target file, resolving any symbolic links in the path.
- `-n`: Displays the target of a symbolic link as is, without resolving it to an absolute path.

For example, if you have a symbolic link named `link_to_somewhere` that points to `/opt/somewhere`, you can run the `readlink` command to view its target like this:

```
readlink link_to_somewhere
```

This will output `/opt/somewhere`.

If you want to view the absolute path of the target file, you can use the `-f` option like this:

```
readlink -f link_to_somewhere
```

This will output the absolute path of the target file, which could be something like `/mnt/disk1/opt/somewhere`. 

## tldr 
 
> Follow symlinks and get symlink information.
> More information: <https://www.gnu.org/software/coreutils/readlink>.

- Get the actual file to which the symlink points:

`readlink {{path/to/file}}`

- Get the absolute path to a file:

`readlink -f {{path/to/file}}`
