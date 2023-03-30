# mount 
## chatgpt 
The "mount" command in Linux is used to mount or attach a file system to a specific directory in the file system. 

When a file system is mounted, it becomes accessible to the system and users can read and write data to it. 

The mount command requires two arguments: the file system to be mounted and the directory where it will be mounted. 

For example, if you have a external hard drive with the file system type of NTFS and you want to mount it at /mnt/external, you would use the following command: 

```
sudo mount -t ntfs /dev/sdb1 /mnt/external
```

In this example, "-t ntfs" tells the mount command the file system type, "/dev/sdb1" is the device file for the external hard drive, and "/mnt/external" is the directory where it will be mounted.

Once the file system is mounted, you can access its contents through the mount point directory. 

You can unmount a file system using the "umount" command followed by the mount point directory. For example: 

```
sudo umount /mnt/external
``` 

Unmounting the file system safely detaches it from the system and ensures data isn't lost. 

## tldr 
 
> Provides access to an entire filesystem in one directory.
> More information: <https://manned.org/mount.8>.

- Show all mounted filesystems:

`mount`

- Mount a device to a directory:

`mount -t {{filesystem_type}} {{path/to/device_file}} {{path/to/target_directory}}`

- Create a specific directory if it does not exist and mount a device to it:

`mount --mkdir {{path/to/device_file}} {{path/to/target_directory}}`

- Mount a device to a directory for a specific user:

`mount -o uid={{user_id}},gid={{group_id}} {{path/to/device_file}} {{path/to/target_directory}}`

- Mount a CD-ROM device (with the filetype ISO9660) to `/cdrom` (readonly):

`mount -t {{iso9660}} -o ro {{/dev/cdrom}} {{/cdrom}}`

- Mount all the filesystem defined in `/etc/fstab`:

`mount -a`

- Mount a specific filesystem described in `/etc/fstab` (e.g. `/dev/sda1 /my_drive ext2 defaults 0 2`):

`mount {{/my_drive}}`

- Mount a directory to another directory:

`mount --bind {{path/to/old_dir}} {{path/to/new_dir}}`
