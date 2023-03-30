# btrbk 
## chatgpt 
btrbk is a command-line utility for managing btrfs snapshots and backups, which are file system snapshots that can be used to restore individual files or entire systems. The command has various options and parameters that can be used to perform different tasks related to the management of btrfs backups.

The basic syntax of the btrbk command is as follows:

btrbk [options]

The options can be used to specify various parameters such as the source, destination, frequency, and retention policy of the backups.

Some common options of the btrbk command are:

- -n or --dry-run: This option allows you to simulate the backup process without making any changes to the file system. It provides a preview of the backup process and outputs the results to the console.

- -c or --config: This option allows you to specify the configuration file for the backup process. The configuration file contains all the settings for the backup process such as the source, destination, frequency, and retention policy.

- -i or --incremental: This option allows you to run an incremental backup, which only backs up the files that have changed since the last backup. This can help to save time and disk space.

- -v or --verbose: This option allows you to display verbose output during the backup process. It provides detailed information about the backup process and the files that are being backed up.

Overall, the btrbk command is a powerful tool for managing btrfs backups, and it can be used to automate the backup process, schedule backups, and create incremental backups. Its flexibility and ease of use make it an essential tool for anyone using the btrfs file system. 

## tldr 
 
> A tool for creating snapshots and remote backups of btrfs subvolumes.
> More information: <https://digint.ch/btrbk/doc/readme.html>.

- Print statistics about configured subvolumes and snapshots:

`sudo btrbk stats`

- List configured subvolumes and snapshots:

`sudo btrbk list`

- Print what would happen in a run without making the displayed changes:

`sudo btrbk --verbose dryrun`

- Run backup routines verbosely, show progress bar:

`sudo btrbk --progress --verbose run`

- Only create snapshots for configured subvolumes:

`sudo btrbk snapshot`
