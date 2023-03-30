# fallocate 
## chatgpt 
fallocate is a command in Linux systems that allows a user to allocate or deallocate space to a file. It is used to manipulate or preallocate space of a file or a range of a file. 

Syntax: 

fallocate [options] file

Options:

1. -l or --length: This option is used to specify the length or size of the space to be allocated or deallocated. This is mandatory when allocating space.

2. -o or --offset: This option is used to specify the starting byte offset of the allocated or deallocated space. This is optional and defaults to zero.

3. -m or --mode: This option is used to specify the mode or permission of the newly created space. This is optional and defaults to the file’s default permission.

4. -n or --keep-size: This option is used to keep the file size before and after allocation unchanged. Any blocks beyond the file size are zeroed.

5. -z or --zero: This option is used to zero the space allocated. 

Examples:

1. To preallocate 1GB space to the file named “example.txt”:

$ sudo fallocate -l 1G example.txt

2. To deallocate the last 100MB space of a file named “example.txt”:

$ sudo fallocate -l -$((100*1024*1024)) example.txt

Note: Negative values for length indicate deallocation.

3. To zero out the allocated space:

$ sudo fallocate -z example.txt

This command will zero out all space allocated to the “example.txt” file. 

In summary, fallocate command is used to provide or remove space to a file in Linux. It has options to set the length, offset, and permission of the allocated space. It can also be used to zero out the allocated space. 

## tldr 
 
> Reserve or deallocate disk space to files.
> The utility allocates space without zeroing.
> More information: <https://manned.org/fallocate>.

- Reserve a file taking up 700 MiB of disk space:

`fallocate --length {{700M}} {{path/to/file}}`

- Shrink an already allocated file by 200 MiB:

`fallocate --collapse-range --length {{200M}} {{path/to/file}}`

- Shrink 20 MB of space after 100 MiB in a file:

`fallocate --collapse-range --offset {{100M}} --length {{20M}} {{path/to/file}}`
