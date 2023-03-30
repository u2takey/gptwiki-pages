# dirs 
## chatgpt 
The `dirs` command is used to display the current list of directories accessed by the user. 

When a user changes the current directory, the path of the previously accessed directory is added to the directory stack. The `dirs` command displays the directory stack in the order of access, starting with the most recent directory.

The output of the `dirs` command displays the directories in a numbered list, where the first entry is the current directory and the remaining entries are the previously accessed directories.

The directory stack is a feature of the shell, so the `dirs` command is available in most Unix-like operating systems, including Linux and macOS. 

## tldr 
 
> Displays or manipulates the directory stack.
> The directory stack is a list of recently visited directories that can be manipulated with the `pushd` and `popd` commands.
> More information: <https://www.gnu.org/software/bash/manual/bash.html#Directory-Stack-Builtins>.

- Display the directory stack with a space between each entry:

`dirs`

- Display the directory stack with one entry per line:

`dirs -p`

- Display only the nth entry in the directory stack, starting at 0:

`dirs +{{N}}`

- Clear the directory stack:

`dirs -c`
