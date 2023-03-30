# diskpart 
## chatgpt 
Diskpart is a command-line utility in Windows that allows users to manage their disk partitions and volumes. It provides advanced functionality for managing disks, allowing users to create, delete, resize, and format partitions. This utility can be useful for advanced users who need to manage their disk space more effectively, or for IT professionals looking to automate disk management tasks.

To use diskpart, you first need to access the Command Prompt by hitting the Windows key and typing in "cmd". Right-click on "Command Prompt" and select "Run as administrator". Once you are in the command prompt, you can enter "diskpart" to start the utility.

After starting diskpart, you will see a command prompt that begins with "DISKPART>". To see a list of all available disks and their associated partitions, you can enter the command "list disk". This will display a table of all the disks attached to the system, including their size, free space, and partition layout.

To select a specific disk to work with, you can use the "select disk" command followed by the disk number. For example, "select disk 0" will select the first disk in the list. Once you have selected a disk, you can then use various commands to create, delete, or manage partitions on that disk.

Some common diskpart commands include:

- create partition primary: This command will create a new primary partition on the selected disk.
- delete partition: This command will delete the currently selected partition.
- format fs=ntfs quick: This command will quickly format the currently selected partition using the NTFS file system.
- extend size=X: This command will extend the current partition by X megabytes (or gigabytes if specified).
- shrink desired=X: This command will shrink the current partition by X megabytes (or gigabytes if specified).

Once you have finished working with diskpart, you can exit the utility by entering the command "exit" or by typing "diskpart /s filename.txt" to execute a script file containing diskpart commands. 

## tldr 
 
> Disk, volume and partition manager.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/diskpart>.

- Run diskpart by itself in an administrative command prompt to enter its command line:

`diskpart`

- List all disks:

`list disk`

- Select a volume:

`select volume {{volume}}`

- Assign a drive letter to the selected volume:

`assign letter {{letter}}`

- Create a new partition:

`create partition primary`

- Activate the selected volume:

`active`

- Exit diskpart:

`exit`
