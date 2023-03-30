# size 
## chatgpt 
The "size" command is a standard Unix command that is used to display the total size (in bytes) of a file in a directory or a group of files in a directory. It is typically used to determine the exact space that a file or group of files is taking up on a disk or in a system.

The syntax of the "size" command is quite simple. You simply need to use the keyword "size" followed by the name of the file or directory that you want to check the size for. For example, the command "size myfile.txt" will display the total size of "myfile.txt" in bytes.

Some important things to note about the "size" command include:

- The size is displayed in bytes by default, but you can use optional flags to display the size in other formats, such as kilobytes (KB), megabytes (MB), or gigabytes (GB).
- If you specify a directory instead of a file, the "size" command will display the total size of all the files in that directory (including any subdirectories).
- If you want to display the sizes of all the files in a directory (without the total), you can use the "ls -l" command followed by the "awk" command to format the output. For example: "ls -l | awk '{print $5, $9}'" will display the sizes and filenames of all the files in the current directory. 

## tldr 
 
> Displays the sizes of sections inside binary files.
> More information: <https://sourceware.org/binutils/docs/binutils/size.html>.

- Display the size of sections in a given object or executable file:

`size {{path/to/file}}`

- Display the size of sections in a given object or executable file in [o]ctal:

`size {{-o|--radix=8}} {{path/to/file}}`

- Display the size of sections in a given object or executable file in [d]ecimal:

`size {{-d|--radix=10}} {{path/to/file}}`

- Display the size of sections in a given object or executable file in he[x]adecimal:

`size {{-x|--radix=16}} {{path/to/file}}`
