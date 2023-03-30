# which 
## chatgpt 
The "which" command is used in Linux and Unix-based operating systems to locate a program or file in the user's environment. It is used to determine the full path of a program that is currently running or installed on the system. 

When the "which" command is executed with the name of a program or file as an argument, it returns the full path to that program or file. For example, if you type "which firefox" in the terminal, the command will return "/usr/bin/firefox" which indicates that the Firefox browser is installed on the system's path "/usr/bin" and can be run from there. 

The "which" command is useful for system administrators to locate the location of important programs installed on their system. It can also be used by developers to ensure that their programs are installed in the correct location and can be accessed by other programs. 

## tldr 
 
> Locate a program in the user's path.
> More information: <https://manned.org/which>.

- Search the PATH environment variable and display the location of any matching executables:

`which {{executable}}`

- If there are multiple executables which match, display all:

`which -a {{executable}}`
