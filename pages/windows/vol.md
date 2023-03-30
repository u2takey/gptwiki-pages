# vol 
## chatgpt 
The "vol" command in Windows is used to show the volume label and serial number of a specified drive or a list of all the drives on the system. It can also display other disk volume information such as the file system type (FAT, NTFS), the cluster size, and the total size and free space available on the drive.

To use the "vol" command, open the Command Prompt window and type "vol" followed by the drive letter or mount point for the desired drive, such as "C:". Alternatively, simply type "vol" without any parameters to display a list of all the drives on the system along with their volume labels and serial numbers.

Example:

To display the volume information for the C: drive, the command would be:

vol C:

This would return information such as the volume label for the C: drive, the serial number, the file system type, and the cluster size.

To display a list of volume information for all the drives on the system, simply type:

vol

This would return a list of all the drives on the system along with their volume labels and serial numbers. 

## tldr 
 
> Display information about volumes.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/vol>.

- Display the label and serial number for the current drive:

`vol`

- Display the label and serial number for a specific volume:

`vol {{D:}}`
