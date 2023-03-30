# mmls 
## chatgpt 
The command "mmls" is a command-line tool in Linux and Unix operating systems that is used to display the layout of partitions on a storage device. It stands for "Master Boot Record (MBR) Partition Table List" command.

The syntax of the "mmls" command is:

mmls [options] device

Where "device" is the name of the storage device you want to display partition information, and "options" are additional parameters or flags that you can pass to the command.

The "mmls" command reads the MBR partition table of the specified device and displays the partition layout in a tabular format. It provides detailed information about the partition start and end sectors, size, and partition type. This information is useful for troubleshooting disk-related issues or partitioning a storage device.

Here are some examples of using the "mmls" command:

1. Display partition information for a disk device:

mmls /dev/sda

2. Display partition information for an image file:

mmls -t dos image.dd

3. Display only active partitions:

mmls -a /dev/sdb

Overall, the "mmls" command is a useful tool for viewing and analyzing partition information on a storage device. 

## tldr 
 
> Display the partition layout of a volume system.
> More information: <https://wiki.sleuthkit.org/index.php?title=Mmls>.

- Display the partition table stored in an image file:

`mmls {{path/to/image_file}}`

- Display the partition table with an additional column for the partition size:

`mmls -B -i {{path/to/image_file}}`

- Display the partition table in a split EWF image:

`mmls -i ewf {{image.e01}} {{image.e02}}`

- Display nested partition tables:

`mmls -t {{nested_table_type}} -o {{offset}} {{path/to/image_file}}`
