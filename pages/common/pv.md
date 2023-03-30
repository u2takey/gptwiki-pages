# pv 
## chatgpt 
The `pv` command in Linux is used to monitor the progress of data as it moves through pipelines. It provides a progress bar, estimated time remaining, current throughput rate, and other statistics related to data transfer. 

The basic syntax of the `pv` command is:

```
pv [OPTIONS] [FILE(s)]
```

Here, `OPTIONS` are the various flags and options that can be used with the command, and `FILE(s)` refers to the input files. If no input file is specified, `pv` takes input from the standard input (stdin).

Some of the commonly used options with `pv` are:

- `-f`: To force `pv` to show progress even if the input is not a regular file (e.g., a device).
- `-L`: To limit the rate of data transfer in bytes/second.
- `-s`: To specify the total size of the input data in bytes.

For example, to monitor the progress of copying a large file called `file.iso` to a USB drive `/dev/sdb`, you can use the following command:

```
pv file.iso > /dev/sdb
```

This will display the progress of data transfer, including the current rate of data transfer, estimated time remaining, and progress bar.

Overall, the `pv` command is useful for monitoring the progress of data transfer and estimating the time required for completion. It can be particularly useful when dealing with large or complex pipelines that involve multiple processes. 

## tldr 
 
> Monitor the progress of data through a pipe.
> More information: <https://manned.org/pv>.

- Print the contents of the file and display a progress bar:

`pv {{path/to/file}}`

- Measure the speed and amount of data flow between pipes (`--size` is optional):

`command1 | pv --size {{expected_amount_of_data_for_eta}} | command2`

- Filter a file, see both progress and amount of output data:

`pv -cN in {{big_text_file}} | grep {{pattern}} | pv -cN out > {{filtered_file}}`

- Attach to an already running process and see its file reading progress:

`pv -d {{PID}}`

- Read an erroneous file, skip errors as `dd conv=sync,noerror` would:

`pv -EE {{path/to/faulty_media}} > image.img`

- Stop reading after reading specified amount of data, rate limit to 1K/s:

`pv -L 1K --stop-at --size {{maximum_file_size_to_be_read}}`
