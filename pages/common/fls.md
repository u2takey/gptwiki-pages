# fls 
## chatgpt 
The "fls" command is a command-line utility that is part of the Sleuth Kit forensic toolkit. It is used for forensically examining the contents of a disk image file or a physical disk itself.

The "fls" command allows forensic investigators to view the contents of a file system, including deleted files and directories without mounting the file system. It does this by using the file system’s metadata to locate files and directories.

The following are the basic syntax and options of the "fls" command:

Syntax:

fls [options] image [inum]

Options:

-о outputs the results in a raw format.
-p shows the full path of the file.
-m shows the mactime of the file.
-r shows the output in recursive form.
-s shows the slack space of the files.
-u shows the unallocated space of the file system.
-i shows the inode information of the files.

Example:

fls -o /path/to/image.dd

The above command will display the raw output of the files and directories present in the disk image.

Overall, "fls" is a useful command for forensic investigators who need to examine the contents of a file system in a forensically sound way. It can help to uncover hidden or deleted files and directories that may be crucial to a forensic investigation. 

## tldr 
 
> List files and directories in an image file or device.
> More information: <https://wiki.sleuthkit.org/index.php?title=Fls>.

- Build a recursive fls list over a device, output paths will start with C:

`fls -r -m {{C:}} {{/dev/loop1p1}}`

- Analyze a single partition, providing the sector offset at which the filesystem starts in the image:

`fls -r -m {{C:}} -o {{sector}} {{path/to/image_file}}`

- Analyze a single partition, providing the timezone of the original system:

`fls -r -m {{C:}} -z {{timezone}} {{/dev/loop1p1}}`
