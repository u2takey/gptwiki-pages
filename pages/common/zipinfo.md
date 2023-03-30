# zipinfo 
## chatgpt 
The `zipinfo` command is used for displaying information about the contents of a zip file.

When you execute the `zipinfo` command followed by the name of a zip file (e.g. `zipinfo myfile.zip`), it will display a list of files and directories contained within the zip file along with their size, date and time of creation, modification and access.

In addition to that, `zipinfo` also provides some advanced features such as listing only files that match specific patterns or displaying information in a detailed format.

Here are some of the most commonly used options with the `zipinfo` command:

- `-h`: Displays the help text and usage information for the `zipinfo` command.
- `-t`: Displays only the list of filenames contained within the zip file.
- `-m`: Displays only the compression method used for each file in the zip archive.
- `-l`: Shows detailed information about each file in the zip archive.
- `-1`: Makes the output list one file per line.
- `-v`: Verbose mode, displays additional information about the zip file, including its compression level, encryption status, etc.

To summarize, the `zipinfo` command is a useful tool for getting information about the contents of a zip file. It provides a quick and easy way to view the list of files and directories within a zip file and their various properties. 

## tldr 
 
> List detailed information about the contents of a `.zip` file.
> More information: <https://manned.org/zipinfo>.

- List all files in a `.zip` file in long format (permissions, ownership, size, and modification date):

`zipinfo {{path/to/archive.zip}}`

- List all files in a `.zip` file:

`zipinfo -1 {{path/to/archive.zip}}`
