# scd 
## chatgpt 
As an AI language model, I assume that the command you meant is "cd" and not "scd" because "scd" is not a known command in most operating systems.

The "cd" command stands for Change Directory, and it is used to navigate between directories (folders) in a command-line interface. By entering "cd" followed by the name of a directory, you can change the current working directory to that directory. For example, if you type "cd Documents" (assuming "Documents" is a folder in your current directory), you will navigate to the "Documents" folder.

Some examples of how to use the "cd" command:

- "cd" - This command will take you to your home directory.
- "cd /" - This command will take you to the root directory.
- "cd ../" - This command will take you up one level in the directory hierarchy.
- "cd ~username/Documents" - This command will take you to the "Documents" folder in the directory of a specific user account.

It's important to note that the "cd" command is specific to command-line interfaces and may not work in graphical user interfaces (GUIs). 

## tldr 
 
> File manager focused on shell integration.
> More information: <https://github.com/cshuaimin/scd>.

- Index paths recursively for the very first run:

`scd -ar {{path/to/directory}}`

- Change to a specific directory:

`scd {{path/to/directory}}`

- Change to a path matching specific patterns:

`scd "{{pattern1 pattern2 ...}}"`

- Show selection menu and ranking of 20 most likely directories:

`scd -v`

- Add a specific alias for the current directory:

`scd --alias={{word}}`

- Change to a directory using a specific alias:

`scd {{word}}`
