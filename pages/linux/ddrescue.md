# ddrescue 
## chatgpt 
The `ddrescue` command is a Linux command-line tool that is primarily used for data recovery and backup purposes. `ddrescue` performs binary copies of data from one block device to another or from a file to a block device. It can also recover data from damaged or corrupted media such as hard disk drives, DVDs, and CDs.

The basic syntax of the `ddrescue` command is:

```
ddrescue [options] infile outfile [logfile]
```

where `infile` is the source file or block device, `outfile` is the destination file or block device, and `logfile` is an optional file that stores the status of the recovery process.

Here are some of the most commonly used options of `ddrescue`:

- `-n`, `--no-scrape`: Zero out unreadable sectors in the destination file instead of trying to read them. This option can save time and prevent further damage to the disk.
- `-r`, `--retrim`: Trim the output file to the size of the successfully recovered data instead of leaving the whole disk space allocated. This option can save disk space.
- `-S`, `--sparse`: Write the output file with sparse blocks. This option can save disk space but may impact performance.
- `-t`, `--timeout`: Set a timeout in seconds for reading from the input file. If the timeout is triggered, `ddrescue` will retry the unreadable sector with smaller and smaller read sizes until it succeeds, or until the minimum read size is reached.
- `-v`, `--verbose`: Output progress information and errors to the terminal. 

Overall, `ddrescue` is a powerful and useful tool for data recovery and backup tasks. However, it requires a good understanding of Linux system administration and careful usage due to the potential impact on disk and data integrity. 

## tldr 
 
> Data recovery tool that reads data from damaged block devices.
> More information: <https://www.gnu.org/software/ddrescue/>.

- Take an image of a device, creating a log file:

`sudo ddrescue {{/dev/sdb}} {{path/to/image.dd}} {{path/to/log.txt}}`

- Clone Disk A to Disk B, creating a log file:

`sudo ddrescue --force --no-scrape {{/dev/sdX}} {{/dev/sdY}} {{path/to/log.txt}}`
