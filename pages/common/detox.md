# detox 
## chatgpt 
Detox is a command-line utility used to clean up filenames. It can be used to remove illegal characters, whitespace, and control characters from filenames. 

The syntax of the command is: 

```
detox [OPTION]... [FILE]...
```

The options available with this command are:

- `-n`: Dry-run mode, which prints out the changes that would be made without actually renaming any files.
- `-v`: Verbose mode, which prints out more detailed information about the changes made to each file.
- `-h`: Displays the help message for the command.

The FILE argument specifies the name of the file(s) to be cleaned up, which can be a single filename, a directory name, or a wildcard pattern. 

When you run the detox command, it will scan the filenames in the specified directory and apply a set of rules to remove illegal characters or whitespace. By default, it will replace spaces with underscores, remove control characters, and convert everything to lowercase letters. If there are any illegal characters in the filename, it will either replace them with a safe character, or remove them altogether. 

Overall, the detox command helps to ensure that all your filenames are clean and properly formatted, making them easier to work with and less likely to cause problems in your filesystem. 

## tldr 
 
> Renames files to make them easier to work with.
> It removes spaces and other such annoyances like duplicate underline characters.
> More information: <https://github.com/dharple/detox>.

- Remove spaces and other undesirable characters from a file's name:

`detox {{path/to/file}}`

- Show how detox would rename all the files in a directory tree:

`detox --dry-run -r {{path/to/directory}}`

- Remove spaces and other undesirable characters from all files in a directory tree:

`detox -r {{path/to/directory}}`
