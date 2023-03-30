# update-alternatives 
## chatgpt 
The `update-alternatives` command is a tool used in Linux operating systems to manage symbolic links which allow multiple versions of a program to co-exist on the same system.

Here's how the command works in detail:

- The command takes an argument in the form of the name of the group of alternatives to be managed. For example, if the command is run as `sudo update-alternatives --config editor`, it will manage the alternatives for the "editor" group.

- The alternatives are defined as symbolic links with a common name in a certain directory. The symbolic links point to the actual executable files that implement the alternatives. For example, if "vi" and "nano" are alternatives for the "editor" group, there will be symbolic links with the names "editor" and "editor.vi" or "editor.nano" in the directory where the command is run.

- The `update-alternatives` command helps manage these alternatives by creating, removing, or updating the symbolic links as needed. For example, if a new alternative is installed, the command can update the symbolic links to include the new alternative as an option.

- The command can also prioritize alternatives, so that the default option for a given group of alternatives can be set. For example, if "nano" is the desired default editor, the command can set the symbolic link for "editor" to point to "nano".

Overall, the `update-alternatives` command is a powerful tool that helps manage multiple versions of software in a Linux system, and allows users to easily switch between different alternatives as needed. 

## tldr 
 
> A convenient tool for maintaining symbolic links to determine default commands.
> More information: <https://manned.org/update-alternatives>.

- Add a symbolic link:

`sudo update-alternatives --install {{path/to/symlink}} {{command_name}} {{path/to/command_binary}} {{priority}}`

- Configure a symbolic link for `java`:

`sudo update-alternatives --config {{java}}`

- Remove a symbolic link:

`sudo update-alternatives --remove {{java}} {{/opt/java/jdk1.8.0_102/bin/java}}`

- Display information about a specified command:

`update-alternatives --display {{java}}`

- Display all commands and their current selection:

`update-alternatives --get-selections`
