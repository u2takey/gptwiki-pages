# velero 
## chatgpt 
Velero is an open-source backup and recovery tool that is specifically designed for cloud-native applications and resources. It is used to backup, migrate, and restore Kubernetes cluster resources and persistent volumes.

The command 'velero' is used to interact with the Velero CLI (Command-Line Interface). The velero command can be used to perform various actions, like creating backups, restoring backups, deleting backups, migrating data, and so on. Here are some of the most frequently used commands with velero:

- 'velero backup create': This command creates a backup of a Kubernetes cluster.

- 'velero backup describe': This command provides detailed information about a specific backup.

- 'velero backup delete': This command deletes a specific backup.

- 'velero restore create': This command restores a backup of a Kubernetes cluster.

- 'velero restore describe': This command provides detailed information about a specific restore.

- 'velero restore delete': This command deletes a specific restore.

- 'velero schedule create': This command creates a backup schedule for a Kubernetes cluster.

- 'velero schedule describe': This command provides detailed information about a specific backup schedule.

- 'velero schedule delete': This command deletes a specific backup schedule.

Some other useful velero commands include 'velero install' (to install Velero on a Kubernetes cluster), 'velero plugin list' (to list the available plugins for Velero), and 'velero version' (to check the installed version of Velero). 

## tldr 
 
> Backup and migrate Kubernetes applications and their persistent volumes.
> More information: <https://github.com/heptio/velero>.

- Create a backup containing all resources:

`velero backup create {{backup_name}}`

- List all backups:

`velero backup get`

- Delete a backup:

`velero backup delete {{backup_name}}`

- Create a weekly backup, each living for 90 days (2160 hours):

`velero schedule create {{schedule_name}} --schedules="{{@every 7d}}" --ttl {{2160h0m0s}}`

- Create a restore from the latest successful backup triggered by specific schedule:

`velero restore create --from-schedule {{schedule_name}}`
