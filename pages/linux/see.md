# see 
## chatgpt 
The "see" command is a command available in most Unix-based operating systems. It is used to display the manual page of the specified command. The syntax of the command is:

see [options] [command]

Where:

- [options]: are various options that modify the behavior of the command. For example, the "-a" option will show all the manual pages that match the command name.
- [command]: is the name of the command for which you want to see the manual page.

When you run the "see" command with a specific command name as an argument, it searches for the corresponding manual page in the system's manual directories and displays it on the terminal screen. Manual pages provide information on the command's usage, syntax, options, and examples.

For example, to see the manual page for the "ls" command, you can type:

see ls

This will display the manual page for the "ls" command on the terminal screen. You can then use various options to navigate the manual page and learn more about the command. 

## tldr 
 
> Alias to `run-mailcap`'s view.
> An alias to a `run-mailcap`'s action print.
> More information: <https://manned.org/see>.

- See action can be used to view any file (usually image) on default mailcap explorer:

`see {{filename}}`

- Using with `run-mailcap`:

`run-mailcap --action=view {{filename}}`
