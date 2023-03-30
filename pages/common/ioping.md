# ioping 
## chatgpt 
ioping is a command-line utility used to measure the input/output operations per second (IOPS) of a disk or file system. It is commonly used in Linux-based systems to assess and troubleshoot disk performance issues.

The syntax of the ioping command is as follows:

```
ioping [options] path
```

The "path" parameter specifies the location of the file or directory for which IOPS are to be measured. If no path is specified, ioping measures the IOPS of the root directory.

Here are some commonly used options with the ioping command:

- `-c`: Specifies the number of I/O requests to send. The default value is 10.
- `-s`: Specifies the size of each I/O request. The default value is 4KB.
- `-w`: Specifies the number of workers to use. The default value is 1.
- `-B`: Displays the result in bytes instead of the default (human-readable) format.

When you execute the ioping command, it sends a series of I/O requests to the specified path or file and records the time it takes to complete each request. Based on these measurements, ioping calculates the IOPS and displays the results on the screen.

For example, if you want to measure the IOPS of the /var/log/ directory with 50 requests and a request size of 8KB, you can use the following command:

```
ioping -c 50 -s 8k /var/log/
```

This will send 50 I/O requests of 8KB each to the /var/log/ directory and display the results in human-readable format. 

## tldr 
 
> Monitor I/O latency in real time.
> More information: <https://github.com/koct9i/ioping>.

- Show disk I/O latency using the default values and the current directory:

`ioping .`

- Measure latency on /tmp using 10 requests of 1 megabyte each:

`ioping -c 10 -s 1M /tmp`

- Measure disk seek rate on `/dev/sdX`:

`ioping -R {{/dev/sdX}}`

- Measure disk sequential speed on `/dev/sdX`:

`ioping -RL {{/dev/sdX}}`
