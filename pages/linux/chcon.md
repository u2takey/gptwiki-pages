# chcon 
## chatgpt 
The command "chcon" is used in Linux-based operating systems to change the security context of files or directories. It stands for "change context." The security context of a file or directory determines the level of access and permissions that are granted to users.

The syntax of the chcon command is as follows: 

chcon [OPTION]... CONTEXT FILE...

The "OPTION" argument specifies any additional options for the command. 

The "CONTEXT" argument specifies the new security context that you want to assign to the files or directories. There are two types of security contexts: 

1. SELinux security contexts: These are used by the Security Enhanced Linux (SELinux) security module to enforce mandatory access control policies. They are specified using a special syntax, as follows: 

user:role:type:level

2. POSIX security contexts: These are used by regular Linux permissions to control a file or directory's access permissions. They are specified using the standard Unix-style permissions, such as "rwxr-xr--".

The "FILE" argument specifies the path to the file or directory that you want to modify.

Some common options used with the chcon command include: 

-R: Modify the security context recursively on all files and directories within a given directory.

-v: Print the name and context of the modified files or directories.

-l: List the available SELinux security contexts.

Overall, the chcon command is a powerful tool for managing file and directory security in Linux-based systems. 

## tldr 
 
> Change SELinux security context of a file or files/directories.
> More information: <https://www.gnu.org/software/coreutils/chcon>.

- View security context of a file:

`ls -lZ {{path/to/file}}`

- Change the security context of a target file, using a reference file:

`chcon --reference={{reference_file}} {{target_file}}`

- Change the full SELinux security context of a file:

`chcon {{user}}:{{role}}:{{type}}:{{range/level}} {{filename}}`

- Change only the user part of SELinux security context:

`chcon -u {{user}} {{filename}}`

- Change only the role part of SELinux security context:

`chcon -r {{role}} {{filename}}`

- Change only the type part of SELinux security context:

`chcon -t {{type}} {{filename}}`

- Change only the range/level part of SELinux security context:

`chcon -l {{range/level}} {{filename}}`
