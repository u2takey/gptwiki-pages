# swapon 
## chatgpt 
The "swapon" command in Linux is used to enable or activate swap space on the system. Swap space is a type of virtual memory that allows the operating system to use a part of the hard disk as additional RAM when the physical memory is full or when a process demands more memory than available. 

The syntax for the "swapon" command is:

swapon [OPTIONS] FILE...

Here, "FILE..." refers to the path of the swap partition or file that needs to be enabled. 

Some common options used with the "swapon" command are:

- -a: Enable all swap space listed in the /etc/fstab file.
- -e: Enable an encrypted swap partition or file.
- -v: Provide verbose output that shows the status of each swap device.

When the "swapon" command is executed, it reads the swap header information of the specified file or partition and makes it available for use by the kernel. The listed swap file/partition is then activated and the system can use it as a form of extended memory. 

It is worth noting that swap space should be used sparingly, as it is slower than RAM and can cause performance issues. If a system frequently relies on swap space, it may be best to upgrade the physical memory (RAM) instead. 

## tldr 
 
> Enables device or file for swapping.
> More information: <https://manned.org/swapon>.

- Get swap information:

`swapon -s`

- Enable a given swap partition:

`swapon {{/dev/sdb7}}`

- Enable a given swap file:

`swapon {{path/to/file}}`

- Enable all swap areas:

`swapon -a`

- Enable swap by label of a device or file:

`swapon -L {{swap1}}`
