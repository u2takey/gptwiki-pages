# dos2unix 
## chatgpt 
The `dos2unix` command is a utility used in Unix and Linux operating systems to convert text files that are created on Windows/DOS machines to Unix/Linux format.

On Windows/DOS systems, lines of text are delimited by a combination of two characters, i.e., a carriage return (CR) followed by a line feed (LF) also known as "\r\n". While in Unix/Linux, lines are separated with only one character, i.e., a line feed (LF) also known as "\n".

When a text file created on a Windows/DOS system is opened on a Unix/Linux system, the presence of the extra carriage return (CR) character can cause issues with the file's display or interpretation by other programs. The `dos2unix` command removes these carriage returns (CR) from the text file to ensure it is compatible with Unix/Linux systems.

The general syntax for the `dos2unix` command is:

```
dos2unix [options] file [file ...]
```

The `options` parameter allows you to specify various options for the command, such as whether to create a backup of the original file or not.

The `file` parameter specifies the name(s) of the file(s) to be converted. You can specify one or more filenames separated by spaces.

Once executed, the `dos2unix` command will open the specified file(s), remove the carriage return characters (CR) present in the file, and save the modified file(s) with the same name. The original file(s) will be overwritten by default, or optionally saved as a backup copy with a ".bak" extension. 

## tldr 
 
> Change DOS-style line endings to Unix-style.
> Replaces CRLF with LF.
> More information: <https://manned.org/dos2unix>.

- Change the line endings of a file:

`dos2unix {{filename}}`

- Create a copy with Unix-style line endings:

`dos2unix -n {{filename}} {{new_filename}}`
