# popd 
## chatgpt 
popd is a command used in Linux and Unix-based operating systems to remove the most recently added directory from the Directory Stack and change the current working directory back to the previously saved directory.

When you use the pushd command, it saves the current directory onto a queue-like data structure called the Directory Stack and changes the current working directory to the specified one. Once a directory is pushed onto the stack, it can be accessed and removed by the popd command.

The syntax of the popd command is as follows:
popd [options]

The options that can be used with popd include:

- -n: popd removes the directory from the stack without changing the current working directory.

- -q: suppresses the output of the current and new directories.

When the popd command is executed without an option, it removes the most recently added directory from the stack and changes the current working directory back to the previous one. 

For example, if the Directory Stack contains directories A, B, and C in the sequence they were added, executing the popd command would remove directory C and change the current working directory to directory B. 

## tldr 
 
> Remove a directory placed on the directory stack via the pushd shell built-in.
> See also `pushd` to place a directory on the stack and `dirs` to display directory stack contents.
> More information: <https://www.gnu.org/software/bash/manual/html_node/Directory-Stack-Builtins.html>.

- Remove the top directory from the stack and cd to it:

`popd`

- Remove the Nth directory (starting from zero to the left from the list printed with `dirs`):

`popd +N`

- Remove the Nth directory (starting from zero to the right from the list printed with `dirs`):

`popd -N`
