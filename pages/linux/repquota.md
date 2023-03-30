# repquota 
## chatgpt 
The `repquota` command is a Linux command used to report on disk usage and limits for the file systems that have disk quotas enabled. 

Here's the brief overview of its functionality: 

- `repquota` is short for "report quota". Quota refers to the limit of space available for users to store data on a filesystem. 
- The command requires root privileges to execute as it deals with system-wide disk usage information.
- The syntax for using `repquota` is `repquota [OPTIONS] FILESYSTEM`. Here, `FILESYSTEM` refers to the mount point of the partition or directory that has quotas enabled. 
- `repquota` generates a report that lists usage and limit information for all the users and groups that have data stored on the specified file system. The report includes the following details: 
  - The user or group ID
  - The amount of disk space used
  - The disk quota limit (if any)
  - The number of files and directories used 
  - The maximum number of files and directories allowed under the quota limit (if any)

Overall, the `repquota` command is primarily used by system administrators to monitor and manage disk usage and quotas for users and groups on a Linux system. 

## tldr 
 
> Display a summary of existing file quotas for a filesystem.
> More information: <https://manned.org/repquota>.

- Report stats for all quotas in use:

`sudo repquota -all`

- Report quota stats for all users, even those who aren't using any of their quota:

`sudo repquota -v {{filesystem}}`

- Report on quotas for users only:

`repquota --user {{filesystem}}`

- Report on quotas for groups only:

`sudo repquota --group {{filesystem}}`

- Report on used quota and limits in a human-readable format:

`sudo repquota --human-readable {{filesystem}}`

- Report on all quotas for users and groups in a human-readable format:

`sudo repquota -augs`
