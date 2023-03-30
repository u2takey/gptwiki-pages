# qmrestore 
## chatgpt 
The `qmrestore` command is used to restore backups that have been taken with the `qmsystem` command in IBM WebSphere MQ. 

When restoring backups, the `qmrestore` command uses the backup_file parameter to specify the file location where the backup is stored. After locating the backup file, `qmrestore` replaces the current queue manager data with the backed-up data. However, it's important to note that if the queue manager is still running, the command will not be able to restore files that are currently in use, and may cause data inconsistencies. 

The `qmrestore` command can also restore only specific objects from backups using various options such as `-r` for restoring ACL information or `-p` for restoring persistent messages. Moreover, the `-e` option is used to remove backups taken by the `qmsystem` command.

Overall, `qmrestore` is a useful command for managing backups and restoring queue manager data if necessary. 

## tldr 
 
> Restore QemuServer vzdump backups.
> More information: <https://pve.proxmox.com/pve-docs/qmrestore.1.html>.

- Restore virtual machine from given backup file on the original storage:

`qmrestore {{path/to/vzdump-qemu-100.vma.lzo}} {{100}}`

- Overwrite existing virtual machine from a given backup file on the original storage:

`qmrestore {{path/to/vzdump-qemu-100.vma.lzo}} {{100}} --force true`

- Restore the virtual machine from a given backup file on specific storage:

`qmrestore {{path/to/vzdump-qemu-100.vma.lzo}} {{100}} --storage {{local}}`

- Start virtual machine immediately from the backup while restoring in the background (only on Proxmox Backup Server):

`qmrestore {{path/to/vzdump-qemu-100.vma.lzo}} {{100}} --live-restore true`
