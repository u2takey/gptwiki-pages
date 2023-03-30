# subst 
## chatgpt 
The `subst` command is a built-in command in the Windows operating system that allows you to create a virtual drive letter that points to a folder or directory on your computer's hard drive. 

The command is used in the following format: 

`subst [drive_letter:][path]`

For example, `subst F: C:\Users\Username\Documents` creates a virtual drive F that is linked to the Documents folder in the user's directory.

When you use the `subst` command, it creates a virtual drive letter and assigns it to the path specified. You can then use this virtual drive letter to access the contents of the folder or directory as if it were a separate physical disk drive.

The virtual drive letter created by the `subst` command is only available for use during the current session or until it is removed manually. To remove a virtual drive created by the `subst` command, simply use the following command:

`subst [drive_letter:] /d`

For example, `subst F: /d` would remove the virtual drive F. 

## tldr 
 
> Associates a path with a virtual drive letter.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/subst>.

- List active associations:

`subst`

- Add an association:

`subst {{Z:}} {{C:\Python2.7}}`

- Remove an association:

`subst {{Z:}} /d`
