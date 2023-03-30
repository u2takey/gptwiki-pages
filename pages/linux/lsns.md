# lsns 
## chatgpt 
The `lsns` command is used to list all currently available namespaces on a Linux system. Namespaces are a Linux kernel feature that allow for the isolation and control of system resources, such as network interfaces, process IDs, and mount points, among others. 

The `lsns` command provides information about each of the available namespaces, including the namespace type (e.g. mount, IPC, network, user, etc.), the inode number of the namespace file in the proc file system, and the number of processes currently inside the namespace.

For example, running the `lsns` command with the `-t net` option will only list network namespaces, while running it with the `-t pid` option will only list process ID namespaces.

The `lsns` command is useful for administrators and developers who need to monitor and manage namespaces on a Linux system. It can also be used in combination with other commands, such as `nsenter` and `unshare`, to enter or create new namespaces for specific tasks or processes. 

## tldr 
 
> List information about all namespaces or about the specified namespace.
> More information: <https://man7.org/linux/man-pages/man8/lsns.8.html>.

- List all namespaces:

`lsns`

- List namespaces in JSON format:

`lsns --json`

- List namespaces associated with {{pid}}:

`lsns --task {{pid}}`

- List the specified type of namespaces only:

`lsns --type <mnt|net|ipc|user|pid|uts|cgroup|time>`

- List namespaces, only showing the namespace ID, type, PID, and command:

`lsns --output NS,TYPE,PID,COMMAND`
