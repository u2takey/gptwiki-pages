# dcfldd 
## chatgpt 
dcfldd is a command-line tool used to write and copy data to and from disks or other input/output sources on Unix and Unix-like systems. Here's an overview of some of the most commonly used parameters:

- if: Specifies the input file or device to read from.
- of: Specifies the output file or device to write to.
- bs: Specifies the block size (in bytes) to use when reading or writing data, e.g. bs=4096.
- hash: Specifies the hash algorithm to use when verifying data integrity, e.g. hash=md5.
- count: Specifies the number of blocks to read or write before stopping.
- conv: Specifies conversion flags to modify the data stream, e.g. conv=noerror,sync.
- progress: Displays progress information during the process.

Here's an example command to create a disk image:

dcfldd if=/dev/sda of=/mnt/external-drive/image.dd bs=512 conv=noerror,sync hash=md5 progress=on

In this command, we're copying the contents of /dev/sda (the first hard disk) to an image file called image.dd on an external drive mounted at /mnt/external-drive. We're using a block size of 512 bytes and the conversion flags noerror and sync to handle errors, and calculating the MD5 hash to verify the integrity of the data being copied. Finally, we're displaying progress information during the process. 

## tldr 
 
> Enhanced version of dd for forensics and security.
> More information: <http://dcfldd.sourceforge.net/>.

- Copy a disk to a raw image file and hash the image using SHA256:

`dcfldd if=/dev/{{disk_device}} of={{file.img}} hash=sha256 hashlog={{file.hash}}`

- Copy a disk to a raw image file, hashing each 1 GB chunk:

`dcfldd if=/dev/{{disk_device}} of={{file.img}} hash={{sha512|sha384|sha256|sha1|md5}} hashlog={{file.hash}} hashwindow={{1G}}`
