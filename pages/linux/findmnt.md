# findmnt 
## chatgpt 
The "findmnt" command is a Linux utility used to display a list of all mounted filesystems on the system. It provides a detailed list of mount points, device and file system type, options, and other relevant information about the mounted file systems. This command works by scanning the "/etc/mtab" file which stores information about currently mounted file systems in the system. The output returned by "findmnt" can be customized using various options, including filtering by file system type, specifying the output format, and printing only certain columns.

Here are some common options available for the "findmnt" command:

- -t: Filter the output based on file system type.
- -o: Specifies the columns to display. The default columns are SOURCE, TARGET, and FSTYPE.
- -n: Print output in a non-tabular format.
- -P: Prints output in a format that can be used as input for the "mount" command.
- -s: Display the output in a summary form.

Overall, the "findmnt" command is a useful tool for identifying mounted file systems and their mounted points on a Linux system. 

## tldr 
 
> Find your filesystem.
> More information: <https://manned.org/findmnt>.

- List all mounted filesystems:

`findmnt`

- Search for a device:

`findmnt {{/dev/sdb1}}`

- Search for a mountpoint:

`findmnt {{/}}`

- Find filesystems in specific type:

`findmnt -t {{ext4}}`

- Find filesystems with specific label:

`findmnt LABEL={{BigStorage}}`
