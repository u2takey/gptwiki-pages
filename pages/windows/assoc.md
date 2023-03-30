# assoc 
## chatgpt 
The `assoc` command is a Windows command-line utility that is used to display, add, or remove file type associations. File type associations are the relationship between a file extension (such as .txt, .docx, .pdf, etc.) and the program that should be used to open that file type.

When used without any arguments, the `assoc` command will display all of the existing file type associations on the system. For example, the command `assoc .txt` will display the file type association for the .txt file extension, which may be something like "txtfile".

To add a new file type association, the `assoc` command is used in combination with the `ftype` command. For example, the following commands will create a new association between the .xyz file extension and a program called "myprogram.exe":

``` 
assoc .xyz=myfiletype
ftype myfiletype=myprogram.exe %1
```

To remove an existing file type association, the `assoc` command can be used with the /d switch, followed by the file extension. For example, the following command will remove the existing association for the .xyz file extension:

```
assoc .xyz /d
```

Overall, the `assoc` command is a powerful tool for managing file type associations in Windows, and can be used to tweak the default programs used to open specific file types. 

## tldr 
 
> Display or change associations between file extensions and file types.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/assoc>.

- List all associations between file extensions and file types:

`assoc`

- Display the associated file type for a specific extension:

`assoc {{.txt}}`

- Set the associated file type for a specific extension:

`assoc .{{txt}}={{txtfile}}`

- View the output of `assoc` one screen at a time:

`assoc | {{more}}`
