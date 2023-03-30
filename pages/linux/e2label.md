# e2label 
## chatgpt 
e2label is a Linux command used to display, set, or change the label of an ext2, ext3, or ext4 file system. The label is a user-defined string that identifies the file system on the storage device, making it easier for users to identify and manage their storage devices. 

Here's a breakdown of the e2label command syntax:

Syntax: `e2label [options] device [label]`

* `options`: Optional. Specifies zero or more command line options that modify the behavior of the command.
* `device`: Required. Specifies the block device or file system for which to display, set, or change the label.
* `label`: Optional. Specifies the new label to set for the file system. If not specified, the command will display the current label.

Some commonly used command options are:

* `-s`: Silent mode. Suppresses all output except error messages.
* `-L`: Set label. Specifies the new label to set for the file system.
* `-n`: Print only the partition name. Suppresses the label and other information.
* `-v`: Verbose mode. Displays detailed output about the operation.


Examples:

1. To display the label of the block device /dev/sda1:

```
e2label /dev/sda1
```

2. To set the label of the block device /dev/sda1 to "MyDisk":

```
e2label /dev/sda1 MyDisk
```

3. To display only the partition name of /dev/sda1:

```
e2label -n /dev/sda1
```

4. To display more detailed output about the operation:

```
e2label -v /dev/sda1
``` 

Note: The e2label command requires root privileges (superuser access) to execute. 

## tldr 
 
> Change the label on an ext2/ext3/ext4 filesystem.
> More information: <https://manned.org/e2label>.

- Change the volume label on a specific ext partition:

`e2label {{/dev/sda1}} "{{label_name}}"`
