# zipgrep 
## chatgpt 
`zipgrep` is a Linux command used to search for text patterns or string within the contents of files compressed in a zip archive. It is a combination of two commands: ZIP and GREP. 

The `zipgrep` command is used to perform searches on the contents of ZIP archives. It can be used to search for a regular expression in one or many files within a ZIP archive. 

Usage: 

```
zipgrep [option(s)] pattern file.zip
```

- `option(s)` is any extra flags that are passed to the command. Some common options are:
    - `-i` case-insensitive search
    - `-h` suppress displaying filenames
    - `-v` display only lines that do not match the pattern
- `pattern` is the text pattern to search for within the compressed files
- `file.zip` is the name of the compressed ZIP archive to search in.

Example:

```
zipgrep -i hello archive.zip
```

This will search for the pattern "hello" in all files within the archive.zip file, ignoring the case of the letters. The command will output any lines that contain the word "hello" and the name of the compressed file where the line is found. 

## tldr 
 
> Find patterns in files in a ZIP archive using extended regular expression (supports `?`, `+`, `{}`, `()` and `|`).
> More information: <https://manned.org/zipgrep>.

- Search for a pattern within a ZIP archive:

`zipgrep "{{search_pattern}}" {{path/to/file.zip}}`

- Print file name and line number for each match:

`zipgrep -H -n "{{search_pattern}}" {{path/to/file.zip}}`

- Search for lines that do not match a pattern:

`zipgrep -v "{{search_pattern}}" {{path/to/file.zip}}`

- Specify files inside a ZIP archive from search:

`zipgrep "{{search_pattern}}" {{path/to/file.zip}} {{file/to/search1}} {{file/to/search2}}`

- Exclude files inside a ZIP archive from search:

`zipgrep "{{search_pattern}}" {{path/to/file.zip}} -x {{file/to/exclude1}} {{file/to/exclude2}}`
