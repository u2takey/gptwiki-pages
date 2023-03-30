# ftype 
## chatgpt 
The 'ftype' command is used in the Windows operating system to display or modify file type associations. It is used to specify the default program that should be used to open a particular file type. 

The command can be used in the Command Prompt window or in Windows PowerShell to display a list of all file types that are associated with specific programs on the computer. It can also be used to modify the default program used for a particular file type.

To display a list of all file types and their associated programs, simply type 'ftype' into the Command Prompt or PowerShell window and press Enter. This will display a list of all file types and the corresponding program that opens them.

To modify the default program used for a specific file type, type 'ftype filetype="program name"' in the Command Prompt or PowerShell window. Replace "filetype" with the file extension of the file type you want to modify, and "program name" with the name of the new program you want to use. For example, to change the default program for opening .txt files to Notepad++, you would enter 'ftype txtfile="C:\Program Files\Notepad++\notepad++.exe" %1' 

Overall, the ftype command is an important tool for managing file associations in the Windows operating system. 

## tldr 
 
> Display or modify file types used for file extension association.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/ftype>.

- Display a list of all file types:

`ftype`

- Display the associated program for a specific file type:

`ftype {{file_type}}`

- Set the associated program for a specific file type:

`ftype {{file_type}}="{{path/to/executable_file}}"`
