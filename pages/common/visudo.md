# visudo 
## chatgpt 
The "visudo" command is used to edit the "/etc/sudoers" file. This file contains the access control rules that determine which users are allowed to run commands with administrative privileges using the "sudo" command. 

When the "visudo" command is executed, it opens the sudoers file in a special editor that provides syntax highlighting and error checking for the contents of the file. This editor is usually "vi", but it can be set to a different editor by changing the "VISUAL" or "EDITOR" environment variable.

Any changes made to the sudoers file using the "visudo" command are subject to syntax checking to ensure they are valid. If there are any errors, "visudo" will not save the changes and will display an error message instead.

It is important to note that the sudoers file must be modified with the "visudo" command, rather than directly editing the file with a text editor. This is because any errors in the sudoers file can potentially render the system unusable by locking out all administrative access, so the syntax checking provided by "visudo" is critical. 

## tldr 
 
> Safely edit the sudoers file.
> More information: <https://www.sudo.ws/docs/man/visudo.man>.

- Edit the sudoers file:

`sudo visudo`

- Check the sudoers file for errors:

`sudo visudo -c`

- Edit the sudoers file using a specific editor:

`sudo EDITOR={{editor}} visudo`

- Display version information:

`visudo --version`
