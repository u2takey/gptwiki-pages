# umount 
## chatgpt 
The `umount` command is used to unmount a mounted file system on Linux or Unix systems. When a file system is mounted, it is attached to a directory in the file system hierarchy, and the files and directories within that directory become accessible. The `umount` command is used to detach the file system from that directory, making it inaccessible.

The syntax of the `umount` command is as follows:

```
umount [options] directory
```

Where `directory` is the mount point for the file system that you want to unmount. The `-v` option can be used to display additional information about the unmounting process.

To unmount a file system, you must have appropriate permission to do so. If the file system is mounted by the root user, you will need to be the root user to unmount it. If the file system is mounted by a non-root user, you must have the appropriate sudo privileges to unmount it.

It is important to note that when you unmount a file system, you should ensure that there are no active processes or open files that are using that file system. When you unmount a file system that is in use, it can cause data loss and file corruption. To avoid this, it is recommended that you close any files or processes that are using the file system before attempting to unmount it. 

## tldr 
 
> Unlink a filesystem from its mount point, making it no longer accessible.
> A filesystem cannot be unmounted when it is busy.
> More information: <https://manned.org/umount.8>.

- Unmount a filesystem, by passing the path to the source it is mounted from:

`umount {{path/to/device_file}}`

- Unmount a filesystem, by passing the path to the target where it is mounted:

`umount {{path/to/mounted_directory}}`

- Unmount all mounted filesystems (except the `proc` filesystem):

`umount -a`
