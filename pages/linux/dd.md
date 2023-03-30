# dd 
## chatgpt 
The "dd" command is a powerful and versatile tool in Linux/Unix-based systems that stands for "data duplicator" or "disk destroyer". It is a command-line utility that allows users to copy and convert data in various ways, and it provides low-level access to storage devices. Here are some of the common usages of the dd command:

1. Disk imaging: The dd command is commonly used to create a byte-to-byte copy of a disk or partition, which is useful for backing up your system or creating images for cloning. Here's an example:

   dd if=/dev/sda of=/backup.img

   This command will copy the entire contents of the /dev/sda drive and save it to a backup image file called backup.img.

2. Creating bootable disks: Another common usage of the dd command is to create a bootable disk from an ISO or IMG image file. Here's an example:

   sudo dd if=/path/to/iso.img of=/dev/sdb bs=4M && sync

   This command will copy the contents of the iso.img to the /dev/sdb disk, which should be your USB disk. The bs parameter sets the block size to 4MB, and the sync command ensures that all data is written to the disk before ejecting.

3. Formatting disks: The dd command can also be used to format disks with various file systems. Here's an example:

   sudo dd if=/dev/zero of=/dev/sdc bs=1M count=10

   This command will write zeros to the first 10MB of the /dev/sdc disk, effectively erasing all existing data and creating a new blank disk with no partition table. You can then use a utility like fdisk to create partitions and format them with a file system.

Overall, the dd command is a powerful and flexible utility that can be used for various data copying and conversion tasks in Linux/Unix-based systems. However, it is also a potentially dangerous tool that can cause data loss if used improperly, so be sure to double-check the parameters before running any dd command. 

## tldr 
 
> Convert and copy a file.
> More information: <https://www.gnu.org/software/coreutils/dd>.

- Make a bootable USB drive from an isohybrid file (such like `archlinux-xxx.iso`) and show the progress:

`dd if={{path/to/file.iso}} of={{/dev/usb_drive}} status=progress`

- Clone a drive to another drive with 4 MiB block, ignore error and show the progress:

`dd if={{/dev/source_drive}} of={{/dev/dest_drive}} bs={{4M}} conv={{noerror}} status=progress`

- Generate a file of 100 random bytes by using kernel random driver:

`dd if=/dev/urandom of={{path/to/random_file}} bs={{100}} count={{1}}`

- Benchmark the write performance of a disk:

`dd if=/dev/zero of={{path/to/file_1GB}} bs={{1024}} count={{1000000}}`

- Generate a system backup into an IMG file and show the progress:

`dd if={{/dev/drive_device}} of={{path/to/file.img}} status=progress`

- Restore a drive from an IMG file and show the progress:

`dd if={{path/to/file.img}} of={{/dev/drive_device}} status=progress`

- Check the progress of an ongoing dd operation (run this command from another shell):

`kill -USR1 $(pgrep ^dd)`
