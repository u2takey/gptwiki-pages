# duplicacy 
## chatgpt 
As an AI language model, I am not able to run a command like duplicacy. However, I can provide the general information that can be useful for you.

Duplicacy is a backup tool that supports cross-platform file and cloud storage backup. It offers incremental and deduplication backups to minimize storage space and optimizing the backup speed. It has a comprehensive command-line interface, using which you can initiate backups, restore data, schedule backups, and monitor the backup logs.

Here are some of the commonly used commands with duplicacy:

- backup [options] [storage_name] [path]: This command initiates a backup of the specified path to the storage location. Options include -hash, which can be used to hash the files before the backup, and -threads, which specifies the number of threads to be used during the backup.

- restore [options] [storage_name] [snap_id] [destination]: This command restores the specified snapshot (snap_id) from the storage location to the specified destination. Options include -hash, which can be used to hash the files before the restore, and -threads, which specifies the number of threads to be used during the restore.

- schedule [options] [storage_name]: This command schedules the backup job at a specific time or interval. Options include -t, which specifies the time to schedule the job, and -interval, which specifies the backup interval.

- list [options] [storage_name]: This command lists all the snapshots available in the storage location. Options include -id, which displays snapshot id, and -t, which displays the time of the snapshot.

- check [options] [storage_name]: This command checks the consistency of the backup data in the storage location. Options include -f, which forces the check to run even if there are no snapshots in storage, and -a, which checks all snapshots in the storage location.

- prune [options] [storage_name]: This command deletes the old snapshots in the storage location to save disk space. Options include -keep, which specifies the number of snapshots to keep, and -exhaustive, which finds all unreferenced chunks in the storage location.

Overall, duplicacy is a feature-rich and efficient backup tool suitable for personal and enterprise-level backup requirements. 

## tldr 
 
> A lock-free deduplication cloud backup tool.
> More information: <https://github.com/gilbertchen/duplicacy/wiki>.

- Use current directory as the repository, initialize a SFTP storage and encrypt the storage with a password:

`duplicacy init -e {{snapshot_id}} {{sftp://user@192.168.2.100/path/to/storage/}}`

- Save a snapshot of the repository to the default storage:

`duplicacy backup`

- List snapshots of current repository:

`duplicacy list`

- Restore the repository to a previously saved snapshot:

`duplicacy restore -r {{revision}}`

- Check the integrity of snapshots:

`duplicacy check`

- Add another storage to be used for the existing repository:

`duplicacy add {{storage_name}} {{snapshot_id}} {{storage_url}}`

- Prune a specific revision of snapshot:

`duplicacy prune -r {{revision}}`

- Prune revisions, keeping one revision every `n` days for all revisions older than `m` days:

`duplicacy prune -keep {{n:m}}`
