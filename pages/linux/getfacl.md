# getfacl 
## chatgpt 
The `getfacl` command is used to retrieve the file access control list (ACL) of a file or directory in a Linux or Unix-based operating system. 

When you run `getfacl` followed by a file or directory name, the command will display the current permissions and ownership settings of that file or folder, including any special permissions or ACL entries that may be assigned.

The output of the `getfacl` command typically includes information on different types of file permissions, such as read, write, execute, and sticky bit permissions, as well as user, group, and other ownership settings. It may also show any other specific ACL entries set on the file.

For instance, the following command can be executed to obtain the access control list of the file named "file.txt":

```
getfacl file.txt
```

This command will produce a list of permissions and access control entries for the "file.txt" file. It is worth noting that the "getfacl" command requires read permissions on the file or directory in order to run successfully. 

## tldr 
 
> Get file access control lists.
> More information: <https://manned.org/getfacl>.

- Display the file access control list:

`getfacl {{path/to/file_or_directory}}`

- Display the file access control list with numeric user and group IDs:

`getfacl -n {{path/to/file_or_directory}}`

- Display the file access control list with tabular output format:

`getfacl -t {{path/to/file_or_directory}}`
