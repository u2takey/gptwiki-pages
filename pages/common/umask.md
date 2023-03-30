# umask 
## chatgpt 
The `umask` command is used to set or view the file mode creation mask. The file mode creation mask is a bit pattern that is used by the operating system to determine the permissions that will be assigned to newly created files and directories.

When you create a new file or directory, the operating system uses the following process to determine the permissions that will be assigned to it:

1. The operating system applies the file mode creation mask to the default permissions for the new file or directory.
2. The resulting permissions are then used to set the actual permissions for the new file or directory.

The `umask` command can be used to set or view the file mode creation mask. The file mode creation mask is specified using a three-digit octal number that represents the mask in binary form.

For example, if the file mode creation mask is set to 022 (octal), this means that the operating system will clear the group and other write bits when creating new files or directories. This results in newly created files and directories having permissions of 644 and 755, respectively.

To view the current file mode creation mask, use the `umask` command without any arguments. For example:

```
$ umask
0022
```

To set the file mode creation mask, use the `umask` command with a three-digit octal number as an argument. For example:

```
$ umask 077
```

This sets the file mode creation mask to 077 (octal), which means that the operating system will clear all group and other permissions when creating new files or directories. This results in newly created files and directories having permissions of 600 and 700, respectively.

The file mode creation mask is usually set in the user's profile file (such as `.bashrc`), which is executed each time the user logs in. This ensures that the file mode creation mask is set to the desired value each time the user creates a new file or directory. 

## tldr 
 
> Manage the read/write/execute permissions that are masked out (i.e. restricted) for newly created files by the user.
> More information: <https://manned.org/umask>.

- Display the current mask in octal notation:

`umask`

- Display the current mask in symbolic (human-readable) mode:

`umask -S`

- Change the mask symbolically to allow read permission for all users (the rest of the mask bits are unchanged):

`umask {{a+r}}`

- Set the mask (using octal) to restrict no permissions for the file's owner, and restrict all permissions for everyone else:

`umask {{077}}`
