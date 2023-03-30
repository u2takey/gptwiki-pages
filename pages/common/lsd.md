# lsd 
## chatgpt 
Unfortunately, as an AI language model, I am not aware of any commonly used command known as "lsd". However, assuming that you meant "ls -d", I can explain that command in detail.

"ls -d" is a command-line utility in Unix-based operating systems, including Linux, macOS, and Unix. It is used to list directories or files in a specified directory without displaying the contents of the subdirectories. The "-d" option stands for "directory," and it tells the "ls" command to limit output to the directory itself and not its contents.

For instance, if you run the command "ls -d /home/user", it will display the details of the directory named "user" within the "/home" directory. If you run the "ls -d" command without specifying any directory, it will display the details of the current working directory.

Overall, "ls -d" is a handy command when you only want to know the details of the targeted directory without showing its subdirectories' contents. 

## tldr 
 
> List directory contents.
> The next generation `ls` command, written in Rust.
> More information: <https://github.com/Peltoche/lsd>.

- List files and directories, one per line:

`lsd -1`

- List all files and directories, including hidden ones, in the current directory:

`lsd -a`

- List all files and directories with trailing `/` added to directory names:

`lsd -F`

- List all files and directories in long format (permissions, ownership, size, and modification date):

`lsd -la`

- List all files and directories in long format with size displayed using human-readable units (KiB, MiB, GiB):

`lsd -lh`

- List all files and directories in long format, sorted by size (descending):

`lsd -lS`

- List all files and directories in long format, sorted by modification date (oldest first):

`lsd -ltr`

- Only list directories:

`lsd -d {{*/}}`
