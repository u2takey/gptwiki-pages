# restic 
## chatgpt 
As an AI language model, I will explain restic as a backup program that is used to backup and restore files and directories on a computer or a network. The restic command is used to interact with the restic program and provides various options to perform backup and restore operations. Some common options that can be used with the restic command include:

- `backup`: This option is used to perform a new backup. Syntax: `restic backup [flags] FILE/FOLDER...`.
- `forget`: This option is used to remove snapshots according to a retention policy. Syntax: `restic forget [flags] [snapshot ID]...`.
- `restore`: This option is used to restore selected files or directories from a backup snapshot. Syntax: `restic restore [flags] [snapshot ID] [FILE/FOLDER]`.
- `check`: This option is used to verify data integrity of backup repository. Syntax: `restic check [flags]`.
- `snapshots`: This option is used to display information about existing backup snapshots. Syntax: `restic snapshots [flags]`.
- `ls`: This option is used to list files and directories in a backup snapshot. Syntax: `restic ls [flags] [snapshot ID] [FILE/FOLDER]`.

Overall, the restic command and its various options make it an effective tool for backup and restore operations, providing users with flexible and efficient means to manage backups on a system. 

## tldr 
 
> A backup program that aims to be fast, secure and efficient.
> More information: <https://restic.net>.

- Initialize a backup repository in the specified local directory:

`restic init --repo {{path/to/repository}}`

- Backup a directory to the repository:

`restic --repo {{path/to/repository}} backup {{path/to/directory}}`

- Show backup snapshots currently stored in the repository:

`restic --repo {{path/to/repository}} snapshots`

- Restore a specific backup snapshot to a target directory:

`restic --repo {{path/to/repository}} restore {{latest|snapshot_id}} --target {{path/to/target}}`

- Restore a specific path from a specific backup to a target directory:

`restic --repo {{path/to/repository}} restore {{snapshot_id}} --target {{path/to/target}} --include {{path/to/restore}}`

- Clean up the repository and keep only the most recent snapshot of each unique backup:

`restic forget --keep-last 1 --prune`
