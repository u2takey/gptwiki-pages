# e2fsck 
## chatgpt 
e2fsck is a command used to check and repair ext2, ext3, and ext4 file systems on Linux operating system. 

The command is typically used to scan a file system to detect errors such as bad blocks, corrupted files, and directory errors, and then attempt to repair those errors. 

The basic syntax of the command is:

e2fsck [options] device

Where "device" is the file system being checked (e.g. /dev/sda1) and "options" are various optional flags, such as:

- -p: Automatically repair errors that can be safely fixed
- -y: Automatically answer yes to all prompts
- -c: Check for bad blocks and add them to the bad block list 
- -f: Force the check even if the file system appears clean
- -n: Do not actually make any changes, just report what would have been done

When using e2fsck, it is important to unmount the file system being checked, or else the command may produce false results or even introduce new errors. 

## tldr 
 
> Check a Linux ext2/ext3/ext4 filesystem. The partition should be unmounted.
> More information: <https://manned.org/e2fsck>.

- Check filesystem, reporting any damaged blocks:

`sudo e2fsck {{/dev/sdXN}}`

- Check filesystem and automatically repair any damaged blocks:

`sudo e2fsck -p {{/dev/sdXN}}`

- Check filesystem in read only mode:

`sudo e2fsck -c {{/dev/sdXN}}`

- Perform an exhaustive, non-destructive read-write test for bad blocks and blacklist them:

`sudo e2fsck -fccky {{/dev/sdXN}}`
