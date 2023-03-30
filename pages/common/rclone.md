# rclone 
## chatgpt 
Rclone is a command-line utility used to manage and sync files across multiple storage services and protocols. It supports a wide range of cloud storage providers such as Google Drive, Amazon S3, Dropbox, Box, Microsoft OneDrive, and many others. 

Some of the commands that can be used with Rclone include:

1. `rclone copy` - used to copy files from one location to another.

2. `rclone sync` - used to synchronize files between two locations, making sure that the files in both locations are the same.

3. `rclone move` - used to move files from one location to another, deleting them from the source location after copying.

4. `rclone delete` - used to delete files from a storage location.

5. `rclone mount` - used to mount a remote storage location in the local file system.

6. `rclone ls` - used to list the files and directories in a storage location.

7. `rclone ncdu` - used to see the disk usage of files and directories in remote storage.

Overall, rclone is a powerful tool that enables easy management and transfer of files across different storage services and protocols. 

## tldr 
 
> CLI program to copy/sync/move files and directories to and from many cloud services.
> More information: <https://rclone.org>.

- List contents of a directory on an rclone remote:

`rclone lsf {{remote_name}}:{{path/to/directory}}`

- Copy file or directory from local source to remote destination:

`rclone copy {{path/to/source_file_or_directory}} {{remote_name}}:{{path/to/destination_directory}}`

- Copy file or directory from remote source to local destination:

`rclone copy {{remote_name}}:{{path/to/source_file_or_directory}} {{path/to/destination_directory}}`

- Sync local source to remote destination, changing the destination only:

`rclone sync {{path/to/file_or_directory}} {{remote_name}}:{{path/to/directory}}`

- Move file or directory from local source to remote destination:

`rclone move {{path/to/file_or_directory}} {{remote_name}}:{{path/to/directory}}`

- Delete remote file or directory (use `--dry-run` to test, remove it to actually delete):

`rclone --dry-run delete {{remote_name}}:{{path/to/file_or_directory}}`

- Mount rclone remote (experimental):

`rclone mount {{remote_name}}:{{path/to/directory}} {{path/to/mount_point}}`

- Unmount rclone remote if CTRL-C fails (experimental):

`fusermount -u {{path/to/mount_point}}`
