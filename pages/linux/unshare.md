# unshare 
## chatgpt 
The `unshare` command is a built-in command of the Linux operating system. It allows a user to create a new namespace or unshare an existing namespace in which a process is running. A namespace is an isolated environment where a process can run with a set of resources or attributes that are different from the rest of the system.

The options for the `unshare` command are:

- `-u` or `--user`: Unshare the user namespace.
- `-i` or `--mount`: Unshare the mount namespace.
- `-n` or `--net`: Unshare the network namespace.
- `-p` or `--pid`: Unshare the process namespace.
- `-U` or `--uts`: Unshare the UTS (Unix Time-sharing System) namespace.

Here's a more detailed explanation of each option:

- `--user`: Unsharing the user namespace means that a process will have its own unique view of user and group IDs. This is useful for running processes with different user permissions than the rest of the system.
- `--mount`: Unsharing the mount namespace means that a process will have its own isolated view of the file system. It can be used for tasks like testing file system features, isolating processes from the rest of the system, or running processes with different mount settings.
- `--net`: Unsharing the network namespace means that a process will have its own isolated networking stack, including IP addresses, routing tables, and network interfaces. This is useful for creating virtual networks, testing network configurations, or running network-intensive processes.
- `--pid`: Unsharing the process namespace means that a process will have its own isolated view of the process ID namespace. This is useful for running processes that need to be isolated from the rest of the system, such as for debugging or testing purposes.
- `--uts`: Unsharing the UTS namespace means that a process will have its own unique view of the system hostname and domain name.

Overall, the `unshare` command is a powerful tool for creating isolated environments within a Linux system, allowing for greater flexibility and security in a variety of use cases. 

## tldr 
 
> Execute a command in new user-defined namespaces.
> More information: <https://www.kernel.org/doc/html/latest/userspace-api/unshare.html>.

- Execute a command without sharing access to connected networks:

`unshare --net {{command}} {{command_arguments}}`

- Execute a command as a child process without sharing mounts, processes, or networks:

`unshare --mount --pid --net --fork {{command}} {{command_arguments}}`
