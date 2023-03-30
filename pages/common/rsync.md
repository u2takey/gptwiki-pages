# rsync 
## chatgpt 
rsync is a command-line tool for efficiently synchronizing files and directories between two locations, whether on a local machine or on remote servers. It is commonly used for backup purposes or for transferring large files between systems.

Here are some of the notable features of rsync:

- It can perform incremental backups, which means that only the changes made to files since the last sync are transferred, reducing network bandwidth consumption and speeding up the process.
- It can copy files both locally and remotely via SSH, and uses encryption to secure the data during transmission.
- It can preserve file ownership, permissions, timestamps, and other attributes during copying, making it particularly useful for maintaining consistent file structures between systems.
- It has a variety of options that allow for customizing the syncing process, such as excluding certain files or directories, compressing files during transfer, and displaying progress indicators.
- It is available on most Unix-like systems, including Linux and macOS.

Here are some examples of how to use the rsync command:

To synchronize the contents of two folders:

```
rsync -av /path/to/folder1/ /path/to/folder2/
```

This will copy all files and subdirectories from folder1 to folder2, preserving all permissions and attributes.

To synchronize files between a local folder and a remote server:

```
rsync -avz /path/to/local/folder/ username@remote.example.com:/path/to/remote/folder/
```

This will transfer all files and subdirectories from the local folder to the specified folder on the remote server, using compression to speed up the process.

To exclude certain files or directories from syncing:

```
rsync -av --exclude '*.txt' /path/to/source/folder/ /path/to/destination/folder/
```

This will exclude all files with a .txt extension from being copied from the source folder to the destination folder. 

## tldr 
 
> Transfer files either to or from a remote host (not between two remote hosts).
> Can transfer single files, or multiple files matching a pattern.
> More information: <https://manned.org/rsync>.

- Transfer file from local to remote host:

`rsync {{path/to/local_file}} {{remote_host}}:{{path/to/remote_directory}}`

- Transfer file from remote host to local:

`rsync {{remote_host}}:{{path/to/remote_file}} {{path/to/local_directory}}`

- Transfer file in [a]rchive (to preserve attributes) and compressed ([z]ipped) mode with [v]erbose and [h]uman-readable [P]rogress:

`rsync -azvhP {{path/to/local_file}} {{remote_host}}:{{path/to/remote_directory}}`

- Transfer a directory and all its children from a remote to local:

`rsync -r {{remote_host}}:{{path/to/remote_directory}} {{path/to/local_directory}}`

- Transfer directory contents (but not the directory itself) from a remote to local:

`rsync -r {{remote_host}}:{{path/to/remote_directory}}/ {{path/to/local_directory}}`

- Transfer a directory [r]ecursively, in [a]rchive to preserve attributes, resolving contained soft[l]inks , and ignoring already transferred files [u]nless newer:

`rsync -rauL {{remote_host}}:{{path/to/remote_directory}} {{path/to/local_directory}}`

- Transfer file over SSH and delete remote files that do not exist locally:

`rsync -e ssh --delete {{remote_host}}:{{path/to/remote_file}} {{path/to/local_file}}`

- Transfer file over SSH using a different port than the default and show global progress:

`rsync -e 'ssh -p {{port}}' --info=progress2 {{remote_host}}:{{path/to/remote_file}} {{path/to/local_file}}`
