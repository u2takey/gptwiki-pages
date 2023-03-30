# fsck 
## chatgpt 
The fsck command stands for "file system consistency check" and it is typically used to verify and repair inconsistencies and errors within a file system. The command performs a scan of the file system's structures and data to identify issues such as broken links, missing files, and incorrect permissions.

When running the fsck command, the user typically specifies the specific file system they wish to check. The command then performs a variety of tests and repairs depending on the specific options used in the command. For example, the user may choose to run a "preen" option, which automatically resolves certain problems without requiring user intervention.

In general, the fsck command is a powerful tool for maintaining the health and integrity of file systems, and it is commonly used by system administrators and advanced users who want to ensure that their file systems are performing optimally. It is important to note, however, that running fsck on a mounted file system can cause data loss or corruption, so users should exercise caution and backup important data before running the command. 

## tldr 
 
> Check the integrity of a filesystem or repair it. The filesystem should be unmounted at the time the command is run.
> More information: <https://manned.org/fsck>.

- Check filesystem `/dev/sdXN`, reporting any damaged blocks:

`sudo fsck {{/dev/sdXN}}`

- Check filesystem `/dev/sdXN`, reporting any damaged blocks and interactively letting the user choose to repair each one:

`sudo fsck -r {{/dev/sdXN}}`

- Check filesystem `/dev/sdXN`, reporting any damaged blocks and automatically repairing them:

`sudo fsck -a {{/dev/sdXN}}`
