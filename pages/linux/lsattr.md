# lsattr 
## chatgpt 
The "lsattr" command is used to list the attributes of files and directories in Linux and Unix. It displays the current attributes of a file or directory, including (but not limited to) flags such as read-only, hidden, immutable, archive, and compressed. 

The syntax of the command is simple - you simply need to type "lsattr" followed by the name of the file or directory you want to view attributes for. If you want to view attributes for all files within a directory, you can include the "-R" option to recursively list all files and subdirectories.

Here are some of the most commonly used options and flags for the "lsattr" command:

- "-a": lists all files, including hidden files, in long format
- "-d": specifies that you want to list the attributes of directories instead of files
- "-R": recursively lists attributes for all files and directories within a specified directory
- "+/-attribute": adds or removes a particular attribute to or from a file or directory. For example, "+i" would set an "immutable" flag, while "-i" would unset it.

Overall, "lsattr" is a useful command for viewing and manipulating file and directory attributes in Linux and Unix systems. 

## tldr 
 
> List file attributes on a Linux filesystem.
> More information: <https://manned.org/lsattr>.

- Display the attributes of the files in the current directory:

`lsattr`

- List the attributes of files in a particular path:

`lsattr {{path}}`

- List file attributes recursively in the current and subsequent directories:

`lsattr -R`

- Show attributes of all the files in the current directory, including hidden ones:

`lsattr -a`

- Display attributes of directories in the current directory:

`lsattr -d`
