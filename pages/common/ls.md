# ls 
## chatgpt 
The "ls" command is used in terminal or command prompt to list the files and directories in the current directory. Here is the detailed explanation of the command:

- "ls" stands for "list"
- By default, "ls" lists the files and directories in the current directory
- The output of the "ls" command shows the name of each file or directory, along with some basic information, such as the file size, permissions, and last modification date
- Options can be added to the "ls" command to modify its behavior. For example, "ls -a" shows hidden files, "ls -l" shows a detailed list with permissions and ownership, and "ls -h" shows the file size in human-readable format
- Multiple directories can be listed by providing their paths as arguments to the "ls" command, like "ls /path/to/directory1 /path/to/directory2"
- The "ls" command can also be used to check if a file or directory exists in the current directory, by specifying its name as an argument. If the file or directory exists, its name will be displayed in the output
- Overall, "ls" is a basic and commonly used command in Unix-like systems, and is useful for exploring the contents of the file system. 

## tldr 
 
> List directory contents.
> More information: <https://www.gnu.org/software/coreutils/ls>.

- List files one per line:

`ls -1`

- List all files, including hidden files:

`ls -a`

- List all files, with trailing `/` added to directory names:

`ls -F`

- Long format list (permissions, ownership, size, and modification date) of all files:

`ls -la`

- Long format list with size displayed using human-readable units (KiB, MiB, GiB):

`ls -lh`

- Long format list sorted by size (descending):

`ls -lS`

- Long format list of all files, sorted by modification date (oldest first):

`ls -ltr`

- Only list directories:

`ls -d */`
