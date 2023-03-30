# mkfs.cramfs 
## chatgpt 
The "mkfs.cramfs" command is used to create a read-only file system in Linux. It is specifically designed for embedded systems and has a compressed file structure, which means that it allows the storage of large files in a highly compressed format. Here are the components and details regarding each part of the command:

- "mkfs" is an abbreviation for "make file system". As the name suggests, it is used to create a new file system on a storage device.
- ".cramfs" refers to the type of file system that is being created. Cramfs stands for "Compressed ROM File System" and is specifically designed for efficient read-only storage of large files.
- Therefore, "mkfs.cramfs" is a command used to make a compressed read-only file system in Linux.

To use the "mkfs.cramfs" command, you need to follow these steps:

1. Open a terminal or command prompt in Linux.
2. Type "mkfs.cramfs" followed by the path to the source files or the directory that is going to be used to build the cramfs file system. For example:

   mkfs.cramfs /dev/source /mnt/cramfs

   In this example, the source files are located in "/dev/source" and the cramfs file system will be mounted in the "/mnt/cramfs" directory.

3. Press Enter to run the command.

Once the command is executed, it will create a compressed read-only file system using the specified source files. The newly created file system can then be mounted and used to access the data stored within it. It's important to note that once a cramfs file system is created, it cannot be modified. Therefore, any changes or updates to data on the file system will require creating a new cramfs file system. 

## tldr 
 
> Creates a ROM filesystem inside a partition.
> More information: <https://manned.org/mkfs.cramfs>.

- Create a ROM filesystem inside partition 1 on device b (`sdb1`):

`mkfs.cramfs {{/dev/sdb1}}`

- Create a ROM filesystem with a volume-name:

`mkfs.cramfs -n {{volume_name}} {{/dev/sdb1}}`
