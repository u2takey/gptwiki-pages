# where 
## chatgpt 
The "where" command is used to locate the executable file associated with a given command or program. When you enter a command in the terminal, the where command searches the directories specified in the PATH environment variable to find the location of the file that contains the executable code for that command.

When you enter a command in the terminal, the shell looks for the specified executable file in each of the directories listed in the PATH environment variable, in the order they are listed. The where command helps you to determine which directory contains the executable file that will be executed when you enter a certain command.

For example, if you type "where ls" in the terminal, the command will search for the "ls" executable file in the directories listed in your PATH environment variable, and print the location(s) of the file(s) on the screen. This can be useful when you have multiple versions of a program installed and need to determine which one is currently being used.

The "where" command is available on both Linux and Windows operating systems. The equivalent commands on Linux are "which" and "type". 

## tldr 
 
> Reports all known instances of a command.
> It could be an executable in the PATH environment variable, an alias, or a shell builtin.
> More information: <https://zsh.sourceforge.io/Doc/Release/Shell-Builtin-Commands.html>.

- Find all instances of a command:

`where {{command}}`
