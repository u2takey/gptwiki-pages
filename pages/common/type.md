# type 
## chatgpt 
The "type" command is a Linux/Unix command that is used to provide information about the type of a given file or command. It is generally used to identify whether the given command is a built-in shell command or an external command. When you use the type command followed by the name of a command, it will display the type of command that has been used.

For example, if you type "type ls" in the terminal, it will display whether the "ls" command is an alias, a shell built-in command, or an external command. Similarly, if you type "type python" in the terminal, it will tell you whether Python is installed on your system, and if so, which version of Python is being used.

The type command also helps distinguish between shell built-in commands and external commands, as built-in shell commands are processed faster than external commands, causing a noticeable difference in execution speed. 

## tldr 
 
> Display the type of command the shell will execute.
> More information: <https://manned.org/type>.

- Display the type of a command:

`type {{command}}`

- Display all locations containing the specified executable:

`type -a {{command}}`

- Display the name of the disk file that would be executed:

`type -p {{command}}`
