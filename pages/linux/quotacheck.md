# quotacheck 
## chatgpt 
quotacheck is a command in Linux systems that checks and corrects inconsistencies in disk quotas. Disk quotas track and limit the amount of disk space and number of files that a user or a group can use on a filesystem.

When you run the quotacheck command with appropriate options and parameters, it scans the specified filesystems for inconsistencies in disk quota data and updates the disk quota files with the appropriate information. If there are any inconsistencies or errors, it fixes them to ensure that the disk quotas are accurate.

The quotacheck command is typically run periodically to ensure that disk quota data stays accurate and up-to-date. To run quotacheck, you need to have root or superuser privileges, as it accesses system files and modifies them.

The basic syntax of the quotacheck command is:

```
quotacheck [options] filesystem
```

Here, `options` are the command-line options that modify the behavior of the command, and `filesystem` specifies the path of the filesystem that you want to check or update the disk quota data.

Some commonly used options of the quotacheck command are:

- `-a`: Runs quotacheck on all filesystems listed in `/etc/fstab`.
- `-m`: Only scans mounted filesystems.
- `-u`: Only scans user quotas.
- `-g`: Only scans group quotas.
- `-v`: Shows verbose output.

For example, to run quotacheck on the `/home` filesystem and update all user and group quotas, you can use the following command:

```
sudo quotacheck -ug /home
```

This will check /home for any inconsistencies in the user and group quotas and update them accordingly. 

## tldr 
 
> Scan a filesystem for disk usage; create, check and repair quota files.
> It is best to run quota check with quotas turned off to prevent damage or loss to quota files.
> More information: <https://manned.org/quotacheck>.

- Check quotas on all mounted non-NFS filesystems:

`sudo quotacheck --all`

- Force check even if quotas are enabled (this can cause damage or loss to quota files):

`sudo quotacheck --force {{mountpoint}}`

- Check quotas on a given filesystem in debug mode:

`sudo quotacheck --debug {{mountpoint}}`

- Check quotas on a given filesystem, displaying the progress:

`sudo quotacheck --verbose {{mountpoint}}`

- Check user quotas:

`sudo quotacheck --user {{user}} {{mountpoint}}`

- Check group quotas:

`sudo quotacheck --group {{group}} {{mountpoint}}`
