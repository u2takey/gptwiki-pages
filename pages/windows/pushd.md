# pushd 
## chatgpt 
The pushd command is a shell command used to change the current directory and also store the current directory in a stack memory for later retrieval. It is mostly used in Unix-based operating systems and in the Windows Command Prompt.

When the pushd command is executed, it adds the current directory to the directory stack memory and then changes the current directory to the specified directory. The stack memory can hold multiple directories and works on a Last-In-First-Out (LIFO) basis, which means the last directory added is the first directory to be retrieved.

Syntax:

pushd [path]

Where “path” is the location of the directory where you want to change the current directory. If no path is specified, it changes the current directory to the root directory.

Once the pushd command is executed, you can use the popd command to retrieve the last added directory and set it as the current directory. The popd command removes the topmost directory from the stack and changes the current directory to the next directory in the stack.

The pushd/popd command is useful when you need to navigate between multiple directories frequently or frequently switch between a few specific directories in a project. By using pushd and popd commands, you can easily switch between directories without having to remember all the path names. 

## tldr 
 
> Place a directory on a stack so it can be accessed later.
> See also `popd` to switch back to original directory.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/pushd>.

- Switch to directory and push it on the stack:

`pushd {{path\to\directory}}`
