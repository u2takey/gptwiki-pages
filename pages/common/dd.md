# dd 
## chatgpt 
The 'dd' command is a utility that can be used for copying and converting data in Unix/Linux operating systems. It is short for 'data duplicator' or 'disk duplicator'. Here are the details of each option and usage of the command:

Syntax: 

```
dd [options] [operands]
```

Options: 

1. if = < input file > - This option specifies the input file to read.
2. of = < output file > -  This option specifies the output file to be created or written to.
3. bs = < blocksize > - This option specifies the block size, which is the number of bytes to read and write at a time.
4. count = < number of blocks > - This option specifies the number of blocks to be read or written.
5. conv = < conversion > - This option specifies the conversion parameters, which can be used for ASCII to EBCDIC conversion, block size conversion, and uppercase to lowercase conversion.
6. seek = < skip blocks > - This option seeks n-blocks before writing (to specify the starting point for writing).
7. iflag = < flags > - Input Flags can be "direct", "dsync", "sync", "fullblock", "noatime", etc.
8. oflag = < flags > - Output Flags can be "direct", "dsync", "sync", "fullblock", "noatime", etc.
9. status = < interval > - This option reports on progress on the copy operation after every n blocks (or records)
10. skip = < skip blocks > - This option skips n-blocks before reading (to specify the starting point for reading).
11. ibs and obs - These options allow you to specify the input and output block sizes (useful for conversions).
12. help – Displays the help screen.

Operands: 

- If no operands are given, dd reads the standard input and writes it to the standard output (useful for testing).
- If an operand is a file name, dd reads or writes to that file.

Usage:

1. Copy the contents of one file to another: 

```
dd if=/inputfile of=/outputfile
```

2. Copy an entire storage device:

```
dd if=/dev/sda of=/dev/sdb
```

3. Copy a section of a device to a file, starting at an offset:

```
dd if=/dev/sda of=~/outputfile bs=1M count=10 skip=100
```

This command reads from /dev/sda, skips the first 100 blocks, reads the next 10 blocks of data (using 1M-block size), and saves the data to ~/outputfile.

4. Create a bootable USB drive from an ISO image:

```
dd if=/path/to/image.iso of=/dev/sdb bs=1M
```

This command writes the contents of /path/to/image.iso to a USB flash drive (/dev/sdb), which can be used for booting a computer.

5. Erasing data on a disk:

```
dd if=/dev/urandom of=/dev/sda bs=1M
```

This command writes random data from /dev/urandom to /dev/sda, which overwrites the existing data on the disk. 

## tldr 
 
> Convert and copy a file.
> More information: <https://www.gnu.org/software/coreutils/dd>.

- Make a bootable USB drive from an isohybrid file (such like `archlinux-xxx.iso`):

`dd if={{path/to/file.iso}} of=/dev/{{usb_drive}}`

- Clone a drive to another drive with 4 MiB block and ignore error:

`dd if=/dev/{{source_drive}} of=/dev/{{dest_drive}} bs={{4194304}} conv={{noerror}}`

- Generate a file of 100 random bytes by using kernel random driver:

`dd if=/dev/urandom of={{path/to/random_file}} bs={{100}} count={{1}}`

- Benchmark the write performance of a disk:

`dd if=/dev/zero of={{path/to/file_1GB}} bs={{1024}} count={{1000000}}`

- Generate a system backup into an IMG file:

`dd if={{/dev/drive_device}} of={{path/to/file.img}}`

- Restore a drive from an IMG file:

`dd if={{path/to/file.img}} of={{/dev/drive_device}}`
