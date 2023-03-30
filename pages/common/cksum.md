# cksum 
## chatgpt 
The 'cksum' command is a UNIX/Linux command that is used to calculate a 32-bit CRC checksum for a file or input. CRC stands for Cyclic Redundancy Check, which is an error-detecting code used to detect accidental changes to raw data.

The syntax of the 'cksum' command is as follows:

```
cksum [OPTIONS] [FILE]
```

where:

- OPTIONS: specify optional flags and parameters for the command.
- FILE: specify the name of the file for which the checksum is to be calculated.

Some of the commonly used options with the 'cksum' command are:

- -b: Generate the checksum in binary format instead of the default hexadecimal format.
- -o: Generate the checksum using the old algorithm instead of the default POSIX algorithm.
- -q: Quiet mode. Suppress the display of filename and file size.

When the 'cksum' command is executed with a file name, it reads the contents of the file and calculates its checksum using the CRC algorithm. The output consists of three columns: the checksum value, the number of bytes in the file and the name of the file. If no file name is specified, 'cksum' reads from the standard input.

The 'cksum' command is used primarily to verify the integrity of files during transmission or storage. It can also be used to compare the contents of two files by comparing their checksum values. 

## tldr 
 
> Calculates CRC checksums and byte counts of a file.
> Note, on old UNIX systems the CRC implementation may differ.
> More information: <https://www.gnu.org/software/coreutils/cksum>.

- Display a 32-bit checksum, size in bytes and filename:

`cksum {{path/to/file}}`
