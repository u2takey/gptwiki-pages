# pushd 
## chatgpt 
The `pushd` command is used to change the current working directory in the command prompt or terminal. It is similar to the `cd` command, but it also maintains a list of previously visited directories, allowing you to easily switch between them.

When you type `pushd` followed by a directory path, the command will change the current directory to that path, and it will also add the previous directory to a stack. This stack keeps track of the directories that you have visited, with the most recent directory being at the top of the stack.

You can use the `popd` command to return to the previous directory on the stack. This will remove the top directory from the stack and change the current directory to the next one down.

Alternatively, you can use the `dirs` command to view the contents of the directory stack. This will show you a list of the directories in the stack, with the most recent directory at the top.

Overall, the `pushd` command is a useful tool for navigating through multiple directories in the command prompt or terminal. It allows you to easily switch between directories and makes it easier to keep track of where you've been. 

## tldr 
 
> Place a directory on a stack so it can be accessed later.
> See also `popd` to switch back to original directory and `dirs` to display directory stack contents.

- Switch to directory and push it on the stack:

`pushd {{path/to/directory}}`

- Switch first and second directories on the stack:

`pushd`

- Rotate stack by making the 5th element the top of the stack:

`pushd +4`
