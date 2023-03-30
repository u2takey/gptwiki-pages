# basename 
## chatgpt 
The `basename` command in Linux is used to extract the filename part from a given path. 

The syntax for the `basename` command is as follows:

```
basename [path] [suffix]
```

`path` is the file path or name which needs to be processed. 

`suffix` is an optional parameter that can be used to remove a specific suffix from the file name. For example, if `suffix` is provided as `.txt`, then the extension `.txt` will be removed from the file name. If this parameter is not provided, the entire file name will be returned.

The `basename` command can be used in several ways, for example, it can be used to:

- Get the file name from a path: `basename /home/user/data/file.txt` will return `file.txt`.
- Get the directory name from a path: `basename /home/user/data/` will return `data`.
- Remove a file extension: `basename file.txt .txt` will return `file`.

It is worth mentioning that the `basename` command does not modify the original file or path; it only returns the processed output. 

## tldr 
 
> Remove leading directory portions from a path.
> More information: <https://www.gnu.org/software/coreutils/basename>.

- Show only the file name from a path:

`basename {{path/to/file}}`

- Show only the rightmost directory name from a path:

`basename {{path/to/directory/}}`

- Show only the file name from a path, with a suffix removed:

`basename {{path/to/file}} {{suffix}}`
