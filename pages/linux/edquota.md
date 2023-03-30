# edquota 
## chatgpt 
The `edquota` command is a Linux/UNIX system command used for editing disk quotas information for users or groups. This command allows system administrators to limit the amount of disk space that a user or a group can use on a file system. When a user or group reaches their allocated quota limit, they will no longer be able to write any new files or data onto the file system.

Here is a breakdown of the `edquota` command and its options:

1. `edquota`: This is the command itself that starts the program.

2. `-u` or `-g <username>`: This option specifies whether the quota should be set for a user or a group. If you use `-u`, you must also provide the username after the option. If you use `-g`, you must provide the group name instead.

3. `-t`: This option is used to set the soft and hard time limits for the user or group, which refers to how long the user or group has to use the space before they are warned or denied access.

4. `-f <filesystem>`: This option specifies the file system to which the user or group quota is being applied.

5. `-p <username>`: This option allows you to copy the quota settings from one user to another.

6. `-h`: This option displays a help screen with all available options for the `edquota` command.

Overall, `edquota` is a useful command for managing disk space usage on a Linux/UNIX system by setting limits for users and groups. 

## tldr 
 
> Edit quotas for a user or group. By default it operates on all filesystems with quotas.
> Quota information is stored permanently in the `quota.user` and `quota.group` files in the root of the filesystem.
> More information: <https://manned.org/edquota>.

- Edit quota of the current user:

`edquota --user $(whoami)`

- Edit quota of a specific user:

`sudo edquota --user {{username}}`

- Edit quota for a group:

`sudo edquota --group {{group}}`

- Restrict operations to a given filesystem (by default edquota operates on all filesystems with quotas):

`sudo edquota --file-system {{filesystem}}`

- Edit the default grace period:

`sudo edquota -t`

- Duplicate a quota to other users:

`sudo edquota -p {{reference_user}} {{destination_user1}} {{destination_user2}}`
