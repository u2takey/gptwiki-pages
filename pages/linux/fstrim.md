# fstrim 
## chatgpt 
The fstrim command is used in Linux systems to discard unused blocks of a file system's flash storage device. This command instructs the Solid State Drive (SSD) or the flash storage device to trim any blocks of data that are no longer in use, thus improving the performance and increasing the lifespan of the storage device. 

The fstrim command is useful when using file systems that support TRIM data command set, such as ext4 or Btrfs. The command can be run manually to trim the entire file system or specific directories that are mounted on an SSD or flash storage device. 

The syntax of the FSTRIM command is as follows: 

fstrim [-hv] [-o offset] [-l length] [-m none|minix|ext2|ext3|ext4|xfs] mountpoint

Here's a brief on each of the options in the fstrim command:

- -h – Shows a help message.
- -v – Provides verbose output during the trimming process.
- -o offset – Identifies the starting offset of the trim operation.
- -l length – Indicates the length of the trim operation.
- -m – Specifies the type of file system to be trimmed.
- mountpoint – Specifies the directory that is mounted on the SSD or flash storage device.

It is important to note that the fstrim command may take a while, depending on the size of the file system and the number of unused blocks that need to be trimmed. It is recommended to run this command periodically to keep the file system optimized. 

## tldr 
 
> Discard unused blocks on a mounted filesystem.
> Only supported by flash memory devices such as SSDs and microSD cards.
> More information: <https://manned.org/fstrim>.

- Trim unused blocks on all mounted partitions that support it:

`sudo fstrim --all`

- Trim unused blocks on a specified partition:

`sudo fstrim {{/}}`

- Display statistics after trimming:

`sudo fstrim --verbose {{/}}`
