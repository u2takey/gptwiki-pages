# rmdir 
## chatgpt 
`rmdir` stands for "remove directory" and is a command used in command-line interfaces to delete an empty directory. 

The syntax of the `rmdir` command is:

```
rmdir [OPTIONS] DIRECTORY
```

`OPTIONS` are the additional flags that make the command do more specific actions or give more information. These are the most commonly used options:

- `-v` (or `--verbose`) - Provides more detailed output while executing the command.

- `-p` (or `--parents`) - Deletes the parent directories which are also empty, using the paths specified in the argument.

- `-ignore-fail-on-non-empty` - Ignores any errors that may occur when trying to delete a non-empty directory.

`DIRECTORY` is the name of the directory that needs to be removed.

It is important to note that `rmdir` can only remove empty directories. If you're trying to delete a directory that contains files or other directories, you need to use the `rm` command along with the `-r` or `-rf` (recursive) option to delete the folder and its contents. It is also important to be careful when using the `rmdir` command as it deletes directories without confirmation or the ability to recover them. 

## tldr 
 
> Remove a directory and its contents.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/rmdir>.

- Remove an empty directory:

`rmdir {{path\to\directory}}`

- Remove a directory and its contents recursively:

`rmdir {{path\to\directory}} /s`

- Remove a directory and its contents recursively without prompting:

`rmdir {{path\to\directory}} /s /q`
