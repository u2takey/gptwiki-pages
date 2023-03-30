# badblocks 
## chatgpt 
badblocks is a Linux command-line utility used to detect bad blocks on a disk device or a partition. Bad blocks are defective areas on the disk that cannot store data correctly. When a bad block is found, the data on that block is lost, and the file system will try to write the data on a different block. The badblocks command is used to scan a storage device to identify these defective sectors and to report them to the operating system so that it can avoid using them. Here's how to use the badblocks command:

Syntax:
```
badblocks [options] device
```

The device argument indicates the block device or partition you want to scan for bad blocks. Usually, this is a hard drive, solid-state drive, or other storage device.

Options:

- **-v**: Verbose mode. Prints detailed output of the scan.
- **-n**: Non-destructive read-write mode. It creates a list of bad blocks without actually writing to them. This option is recommended because it won't damage any data that's currently on the device.
- **-w**: Destructive read-write mode. It scans the device and writes patterns to the bad blocks, which marks them as bad and prevents the operating system from using them. This option is not recommended because it can cause data loss.
- **-p**: Specifies the block size that should be scanned.
- **-o**: Specifies the output file to write the results to.
- **-s**: Shows the progress of the scan.

After starting the badblocks command, it will scan the specified device for bad blocks. The output will list the blocks that are found to be bad. If the scan finds any bad blocks, it's recommended to replace the device with a new one. 

## tldr 
 
> Search a device for bad blocks.
> Some usages of badblocks can cause destructive actions, such as erasing all data on a disk, including the partition table.
> More information: <https://manned.org/badblocks>.

- Search a disk for bad blocks by using a non-destructive read-only test:

`sudo badblocks {{/dev/sdX}}`

- Search an unmounted disk for bad blocks with a non-destructive read-write test:

`sudo badblocks -n {{/dev/sdX}}`

- Search an unmounted disk for bad blocks with a destructive write test:

`sudo badblocks -w {{/dev/sdX}}`

- Search an unmounted disk for bad blocks with a destructive write test and show verbose status:

`sudo badblocks -svw {{/dev/sdX}}`

- Search an unmounted disk in destructive mode and output found blocks to a file:

`sudo badblocks -o {{path/to/file}} -w {{/dev/sdX}}`

- Search an unmounted disk in destructive mode with improved speed using 4K block size and 64K block count:

`sudo badblocks -w -b {{4096}} -c {{65536}} {{/dev/sdX}}`
