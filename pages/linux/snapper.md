# snapper 
## chatgpt 
Snapper is a command-line tool in Linux that is used to manage Btrfs filesystems, which is a copy-on-write filesystem used for Linux. Btrfs is a modern filesystem that supports advanced features such as snapshotting, which allows the system to take a snapshot of the filesystem at a specific point in time. 

Snapper allows users to manage these snapshots by creating, deleting, and restoring them. It also allows users to compare snapshots to see what files have changed. It helps users to manage the size of the snapshot and keep their filesystem organized.

Some common commands used with snapper are:

1. snapper create - This command creates a new snapshot of the filesystem.

2. snapper delete - This command deletes a specified snapshot.

3. snapper list - This command lists all available snapshots.

4. snapper rollback - This command rolls back the filesystem to a specified snapshot.

5. snapper diff - This command compares two snapshots to show the differences.

Overall, snapper is a useful tool for managing Btrfs filesystems and allows users to manage their files and system more efficiently. 

## tldr 
 
> Filesystem snapshot management tool.
> More information: <http://snapper.io/manpages/snapper.html>.

- List snapshot configs:

`snapper list-configs`

- Create snapper config:

`snapper -c {{config}} create-config {{path/to/directory}}`

- Create a snapshot with a description:

`snapper -c {{config}} create -d "{{snapshot_description}}"`

- List snapshots for a config:

`snapper -c {{config}} list`

- Delete a snapshot:

`snapper -c {{config}} delete {{snapshot_number}}`

- Delete a range of snapshots:

`snapper -c {{config}} delete {{snapshot_X}}-{{snapshot_Y}}`
