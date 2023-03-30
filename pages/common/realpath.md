# realpath 
## chatgpt 
The `realpath` command is a utility in Linux and Unix systems that returns the absolute path of a file or directory. It resolves all symbolic links and "." and ".." references in the path and returns the fully resolved and canonicalized path.

The syntax for using the `realpath` command is as follows:

```
realpath [options] file/dir-path
```

Options may include:

- `--help`: Display a help message and exit.
- `-m`: Do not resolve symlinks.
- `-q`: Quiet mode, suppresses error messages.

The `file/dir-path` argument represents the file or directory path to be resolved. If the path is relative, `realpath` will make it absolute by appending it to the current working directory.

Here's an example of using the `realpath` command to get the absolute path of a file:

```
$ realpath file.txt
/home/user/documents/file.txt
```

In this example, `realpath` returned the absolute path of the file `file.txt` in the `documents` directory located under the home directory of the user.

If there are any symbolic links or "." and ".." references in the file or directory path, `realpath` will resolve them and return the fully resolved path. 

## tldr 
 
> Display the resolved absolute path for a file or directory.
> More information: <https://www.gnu.org/software/coreutils/realpath>.

- Display the absolute path for a file or directory:

`realpath {{path/to/file_or_directory}}`

- Require all path components to exist:

`realpath --canonicalize-existing {{path/to/file_or_directory}}`

- Resolve ".." components before symlinks:

`realpath --logical {{path/to/file_or_directory}}`

- Disable symlink expansion:

`realpath --no-symlinks {{path/to/file_or_directory}}`

- Suppress error messages:

`realpath --quiet {{path/to/file_or_directory}}`
