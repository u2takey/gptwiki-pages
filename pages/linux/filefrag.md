# filefrag 
## chatgpt 
The "filefrag" command in Linux is used to display the fragmentation details of a file. The command takes a single argument, which is the name of the file for which the fragmentation details are to be displayed. 

The output of the command includes the number of fragments for the given file, the size of each fragment, the starting offset of each fragment, and the file system block number of each fragment. 

Some common options that can be used with the "filefrag" command are:

- "-v" or "--verbose": This option increases the verbosity of the output and provides more detailed information about the fragmentation of the file.
- "-b" or "--block-size": This option specifies the block size to be used for displaying the output. By default, the block size is set to 1KB.
- "-e" or "--extents": This option displays the fragmentation information for each extent of the file separately.

Overall, the "filefrag" command is a useful tool for analyzing the fragmentation of files in Linux file systems, which can help in optimizing file access and improving system performance. 

## tldr 
 
> Report how badly fragmented a particular file might be.
> More information: <https://manned.org/filefrag>.

- Display a report for a specific file:

`filefrag {{path/to/file}}`

- Display a report for space-separated list of files:

`filefrag {{path/to/file1}} {{path/to/file2}}`

- Display a report using a 1024 byte blocksize:

`filefrag -b {{path/to/file}}`

- Sync the file before requesting the mapping:

`filefrag -s {{path/to/files}}`

- Display mapping of extended attributes:

`filefrag -x {{path/to/files}}`

- Display a report with verbose information:

`filefrag -v {{path/to/files}}`
