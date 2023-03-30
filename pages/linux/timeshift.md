# timeshift 
## chatgpt 
Timeshift is a command-line tool that is used to create and restore system snapshots in Linux operating systems. System snapshots are a point-in-time copy of the entire system and can be used to restore the system to a working state if anything goes wrong. It uses the file system’s capability of creating hard links to take the snapshot of a system.

This tool is installed by default on some Linux distributions like Linux Mint, Ubuntu, and Fedora but for most others, you have to install it manually.

Once installed, you can open the Timeshift application from the menu or run it from the command line using the "timeshift" command followed by the command options.

The command options include:

- "--create" - Create a system snapshot.
- "--list" - See a list of available snapshots.
- "--restore" - Restore your system to a previous snapshot.
- "--delete" - Delete a specific snapshot.
- "--rsync" - Use rsync instead of Btrfs to create snapshots.
- "--snapshot-device" - Specify the device to create and store snapshots on.
- "--snapshot-size" - Specify the size of snapshots to create.

Here are some examples of using Timeshift command:

To create a snapshot: 

sudo timeshift --create

To restore a previous snapshot:

sudo timeshift --restore

To delete a specific snapshot:

sudo timeshift --delete  "Snapshot-Name"

To see a list of available snapshots:

sudo timeshift --list

That's it! These are the basic commands and options you can use with Timeshift. With this tool, you can easily create and restore system backups and keep your system safe from any unexpected situations. 

## tldr 
 
> System restore utility.
> More information: <https://github.com/teejee2008/timeshift>.

- List snapshots:

`sudo timeshift --list`

- Create a new snapshot (if scheduled):

`sudo timeshift --check`

- Create a new snapshot (even if not scheduled):

`sudo timeshift --create`

- Restore a snapshot (selecting which snapshot to restore interactively):

`sudo timeshift --restore`

- Restore a specific snapshot:

`sudo timeshift --restore --snapshot '{{snapshot}}'`

- Delete a specific snapshot:

`sudo timeshift --delete --snapshot '{{snapshot}}'`
