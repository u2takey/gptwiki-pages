# fsutil 
## chatgpt 
Fsutil is a Windows command-line tool that is used to manage and query various file system related operations. It provides a wide range of file system utility functions, including managing drive letters, allocating and deallocating disk space, creating, deleting and renaming a file or folder, querying various file system properties, creating and managing hard links and junctions, formatting disk partitions, managing file and folder compression, and much more. 

The fsutil command is used in combination with specific parameters depending on the task at hand. For example, to create a hard link, the following command can be used:

`fsutil hardlink create <ExistingFile> <NewFileName>`

where `<ExistingFile>` is the original file you want to link to, and `<NewFileName>` is the name you want to give to the new link. 

Similarly, to format a disk partition, the following command can be used:

`fsutil.exe volume diskformat <DriveLetter> /FS:<FileSystemType>`

where `<DriveLetter>` is the letter of the drive you want to format, and `<FileSystemType>` is the type of file system you want to create, such as NTFS, exFAT, FAT, etc.

Overall, fsutil is a powerful and versatile tool that provides extensive file system management capabilities, making it an essential utility for system administrators and power users. 

## tldr 
 
> Displays information about file system volumes.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/fsutil>.

- Display a list of volumes:

`fsutil volume list`

- Display information about a volume's file system:

`fsutil fsInfo volumeInfo {{drive_letter|volume_path}}`

- Display the current state of the file system auto-repair for all volumes:

`fsutil repair state`

- Display the dirty bit state of all volumes:

`fsutil dirty query`

- Set the dirty bit state of a volume:

`fsutil dirty set {{drive_letter|volume_path}}`
