# mount 
## chatgpt 
"mount" is a command used in Linux and other UNIX-based operating systems to attach a file system or a device (such as a CD-ROM or USB drive) to a specific directory location in the filesystem hierarchy. 

The syntax of the mount command is:

```
mount [-lhV] [-o options] [-t fstype] device|dir mountpoint
```

Here is a brief explanation of the parameters used in the mount command:

* -l: Shows all mounted file systems.
* -h: Displays a help message that explains the usage of the "mount" command.
* -V: Prints the version of the "mount" command.
* -o: Allows you to specify certain options that govern the behavior of the mount command.
* -t: Specifies the file system type of the device. If not specified, the "mount" command will attempt to detect the file system type automatically.
* device|dir: Specifies the device or directory that you want to mount.
* mountpoint: The path to the directory where you want to mount the device.

For example, to mount a USB drive, you would enter the command:

```
sudo mount /dev/sdb1 /mnt/usb
```

This command tells Linux to mount the device located at /dev/sdb1 (which is typically the device ID of the USB drive) onto the directory /mnt/usb. The "sudo" prefix is used to run the mount command as the system superuser, which is necessary for some devices that require extra privileges to mount. 

Once mounted, the files and directories on the USB drive will be accessible through the /mnt/usb directory for reading or writing. 

It's important to remember to unmount the device before disconnecting it to prevent data loss or file system corruption. You can use the "umount" command to safely unmount the device. 

## tldr 
 
> Mount Network File System (NFS) network shares.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/mount>.

- Mount a share to the "Z" drive letter:

`mount \\{{computer_name}}\{{share_name}} {{Z:}}`

- Mount a share to the next available drive letter:

`mount \\{{computer_name}}\{{share_name}} *`

- Mount a share with a read timeout in seconds (defaults to 0.8, can be 0.9 or 1 to 60):

`mount -o timeout={{seconds}} \\{{computer_name}}\{{share_name}} {{Z:}}`

- Mount a share and retry up to 10 times if it fails:

`mount -o retry={{retries}} \\{{computer_name}}\{{share_name}} {{Z:}}`

- Mount a share with forced case sensitivity:

`mount -o casesensitive \\{{computer_name}}\{{share_name}} {{Z:}}`

- Mount a share as an anonymous user:

`mount -o anon \\{{computer_name}}\{{share_name}} {{Z:}}`

- Mount a share using a specific mount type:

`mount -o mtype={{soft|hard}} \\{{computer_name}}\{{share_name}} {{Z:}}`
