# cmd 
## chatgpt 
"cmd" is a command used in Windows operating system which stands for Command Prompt. When this command is executed, it opens up a new window that allows the user to execute various commands and perform actions related to the system. The Command Prompt provides a text-based interface where the user can type in commands and receive feedback in the form of text messages. 

Some of the common tasks that can be performed using the Command Prompt include file management, network diagnosis, system configuration, and troubleshooting. The Command Prompt provides a powerful set of tools and commands that can be used to perform complex tasks and automate processes.

To use the Command Prompt, simply click on the Start button, type "cmd" in the search box, and press Enter. This will open up the Command Prompt window. From here, the user can type in commands and hit Enter to execute them. Some examples of basic commands include "dir" to list the contents of a directory, "cd" to change the current directory, and "ipconfig" to display the network configuration information. 

## tldr 
 
> The Windows command interpreter.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/cmd>.

- Start an interactive shell session:

`cmd`

- Execute specific [c]ommands:

`cmd /c {{echo Hello world}}`

- Execute a specific script:

`cmd {{path\to\script.bat}}`

- Execute specific commands and then enter an interactive shell:

`cmd /k {{echo Hello world}}`

- Start an interactive shell session where `echo` is disabled in command output:

`cmd /q`

- Start an interactive shell session with delayed [v]ariable expansion enabled or disabled:

`cmd /v:{{on|off}}`

- Start an interactive shell session with command [e]xtensions enabled or disabled:

`cmd /e:{{on|off}}`

- Start an interactive shell session with used [u]nicode encoding:

`cmd /u`
