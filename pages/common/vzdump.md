# vzdump 
## chatgpt 
The `vzdump` command is a tool used to create backups of OpenVZ containers. It comes bundled with the OpenVZ software and is used to create full backups of a container's file system, configuration files, and metadata. The `vzdump` command has a number of options that can be used to customize the backup process, including the ability to specify the target file format (such as tar or tar.gz), the location of the backup file, and the inclusion or exclusion of specific files or directories.

To run the `vzdump` command, you must have root access to the OpenVZ server. The basic syntax for the command is as follows:

```
vzdump [OPTIONS] CTID
```

The `OPTIONS` parameter can be used to specify various options for the backup, such as the backup format, compression type, and file location. The `CTID` parameter is the ID of the container you want to back up.

For example, to create a backup of container #101 in tar.gz format and save it to the /backup directory, you would use the following command:

```
vzdump --compress gzip --dumpdir /backup 101
```

This would create a backup file named something like `vzdump-101.tar.gz` in the `/backup` directory.

In addition to creating backups, the `vzdump` command can also be used to restore backups or migrate containers to other servers. However, these processes require additional configuration and setup beyond the basic backup command. 

## tldr 
 
> Backup Utility for virtual machines and containers.
> More information: <https://pve.proxmox.com/pve-docs/vzdump.1.html>.

- Dump a guest virtual machine into the default dump directory (usually `/var/lib/vz/dump/`), excluding snapshots:

`vzdump {{vm_id}}`

- Back up the guest virtual machines with the IDs 101, 102, and 103:

`vzdump {{101 102 103}}`

- Dump a guest virtual machine using a specific mode:

`vzdump {{vm_id}} --mode {{suspend|snapshot}}`

- Back up all guest systems and send an notification email to the root and admin users:

`vzdump --all --mode {{suspend}} --mailto {{root}} --mailto {{admin}}`

- Use snapshot mode (no downtime required) and a non-default dump directory:

`vzdump {{vm_id}} --dumpdir {{path/to/directory}} --mode {{snapshot}}`

- Back up all guest virtual machines excluding the IDs 101 and 102:

`vzdump --mode {{suspend}} --exclude {{101, 102}}`
