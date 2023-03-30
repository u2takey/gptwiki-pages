# attrib 
## chatgpt 
The attrib command is a Windows command used to display or modify the attributes of a file or folder. 

Syntax:

attrib [+/− attribute] [filepath]

The possible arguments for attributes are as follows:

- r: Read-only attribute
- a: Archive attribute
- s: System attribute
- h: Hidden attribute

The “+” sign is used to add attributes to the file or folder while the “-” sign is used to remove attributes from the file or folder. 

For example, to add the hidden attribute to a file named “example.txt”, the command would be:

attrib +h example.txt

To remove the read-only attribute from a file named “example.docx”, the command would be:

attrib -r example.docx

If you run the attrib command without any arguments, it will display the current attributes of the file or folder. 

Note that some attributes cannot be removed from certain files, such as system files or read-only files. Also, modifying the attributes of critical system files may cause system instability or malfunction. Therefore, it is recommended to use caution when using the attrib command. 

## tldr 
 
> Display or change attributes of files or directories.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/attrib>.

- Display all set attributes of files in the current directory:

`attrib`

- Display all set attributes of files in a specific directory:

`attrib {{path\to\directory}}`

- Display all set attributes of files and [d]irectories in the current directory:

`attrib /d`

- Display all set attributes of files in the current directory and [s]ub-directories:

`attrib /s`

- Add the `[r]ead-only` or `[a]rchive` or `[s]ystem` or `[h]idden` or `not content [i]ndexed` attribute to files or directories:

`attrib +{{r|a|s|h|i}} {{path\to\file_or_directory1 path\to\file_or_directory2 ...}}`

- Remove a specific attribute of files or directories:

`attrib -{{r|a|s|h|i}} {{path\to\file_or_directory1 path\to\file_or_directory2 ...}}`
