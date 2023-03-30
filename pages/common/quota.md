# quota 
## chatgpt 
The "quota" command is a system administration command for checking and managing disk quotas on a Linux or Unix system. It is used to set, edit, and report disk usage quotas for users, groups, and file systems. 

When used without any options or arguments, the "quota" command will display the current disk usage and quota limits for the logged-in user. This includes the amount of disk space used, the quota limit, and the percentage of usage. 

The "quota" command can also be used to check the quotas for a specific user or group by specifying the name. It can also be used to report the quota status for all users, using the "-u" option, or for all file systems, using the "-f" option. 

To set or modify disk quotas, the "quota" command can be used along with the "edquota" command. This allows the system administrator to set quotas for individual users or groups, as well as assign soft and hard limits for disk usage. 

Overall, the "quota" command is a useful tool for maintaining disk space usage on a Linux or Unix system and ensuring that users and groups do not exceed their allotted storage quotas. 

## tldr 
 
> Display users' disk space usage and allocated limits.
> More information: <https://manned.org/quota>.

- Show disk quotas in human-readable units for the current user:

`quota -s`

- Verbose output (also display quotas on filesystems where no storage is allocated):

`quota -v`

- Quiet output (only display quotas on filesystems where usage is over quota):

`quota -q`

- Print quotas for the groups of which the current user is a member:

`quota -g`

- Show disk quotas for another user:

`sudo quota -u {{username}}`
