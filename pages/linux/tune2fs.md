# tune2fs 
## chatgpt 
The "tune2fs" command is a utility in Linux-based operating systems that allows users to adjust various parameters and settings related to the ext2, ext3, and ext4 file systems. Here is a breakdown of some of the most common options and arguments that can be used with this command:

- "-c": Sets the maximum mount count between two file system checks. For example, "tune2fs -c 10 /dev/sdb1" would configure the file system on /dev/sdb1 to be checked every 10 mounts.
- "-e": Configures the behavior of the file system when it encounters an error. By default, the file system will enter read-only mode if it encounters an error. This option allows users to change that behavior. For example, "tune2fs -e continue /dev/sdb1" would configure the file system on /dev/sdb1 to continue operating even if it encounters errors.
- "-j": Enables the creation of an ext3 journal on the file system's device. For example, "tune2fs -j /dev/sdb1" would create a journal for the file system on /dev/sdb1.
- "-l": Prints out the file system's current settings and parameters. For example, "tune2fs -l /dev/sdb1" would show the current settings for the file system on /dev/sdb1.
- "-m": Configures the percentage of the file system that is reserved for the root user to prevent the file system from becoming completely full. For example, "tune2fs -m 5 /dev/sdb1" would set aside 5% of the file system on /dev/sdb1 for the root user.
- "-r": Configures the default mount option for the file system. For example, "tune2fs -r 0 /dev/sdb1" would prevent the file system on /dev/sdb1 from being mounted automatically.
- "-U": Sets the UUID of the file system. For example, "tune2fs -U 12345678-9abc-def0-1234-56789abcdef0 /dev/sdb1" would set the UUID of the file system on /dev/sdb1 to the specified value.

These are just a few examples of the options and arguments that can be used with the "tune2fs" command. Users can refer to the command's documentation or help files for more information on how to use it. 

## tldr 
 
> Adjust parameters of an ext2, ext3 or ext4 filesystem.
> May be used on mounted filesystems.
> More information: <https://manned.org/tune2fs>.

- Set the max number of counts before a filesystem is checked to 2:

`tune2fs -c {{2}} {{/dev/sdXN}}`

- Set the filesystem label to MY_LABEL:

`tune2fs -L {{'MY_LABEL'}} {{/dev/sdXN}}`

- Enable discard and user-specified extended attributes for a filesystem:

`tune2fs -o {{discard,user_xattr}} {{/dev/sdXN}}`

- Enable journaling for a filesystem:

`tune2fs -o^{{nobarrier}} {{/dev/sdXN}}`
