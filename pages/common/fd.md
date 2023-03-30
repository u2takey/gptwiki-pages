# fd 
## chatgpt 
The `fd` command is a Linux command-line utility that is used to find and list open files and directories. Here's a detailed explanation of the command:

Syntax:
```
fd [options] [path...]
```

Options:
- `-a` or `--all`: Display both regular and special files.
- `-d` or `--directory`: Display directories only.
- `-e` or `--exclude`: Exclude the specified pattern from the search.
- `-H` or `--hidden`: Search hidden files and directories.
- `-I` or `--ignore-case`: Search without case sensitivity.
- `-L` or `--follow`: Follow symbolic links.
- `-t` or `--type`: Limit search to specific file type (e.g. f for file, d for directory).

Arguments:
- `path...`: The path (or paths) to search for open files and directories.

Example usage:

1. Display all open files:
```
fd
```

2. Display only open directories:
```
fd -d
```

3. Exclude PDF files from the search:
```
fd -e pdf
```

4. Search for hidden files/directories:
```
fd -H
```

5. Search for all symbolic links (including broken ones):
```
fd -L -t l
```

The `fd` command is a very versatile tool for finding and managing open files and directories on a Linux system. It can be combined with other command-line utilities to perform more complex tasks, making it a powerful and valuable tool for system administrators and developers. 

## tldr 
 
> An alternative to `find`.
> Aims to be faster and easier to use than `find`.
> More information: <https://github.com/sharkdp/fd>.

- Recursively find files matching a specific pattern in the current directory:

`fd "{{string|regex}}"`

- Find files that begin with `foo`:

`fd "^foo"`

- Find files with a specific extension:

`fd --extension txt`

- Find files in a specific directory:

`fd "{{string|regex}}" {{path/to/directory}}`

- Include ignored and hidden files in the search:

`fd --hidden --no-ignore "{{string|regex}}"`

- Execute a command on each search result returned:

`fd "{{string|regex}}" --exec {{command}}`
