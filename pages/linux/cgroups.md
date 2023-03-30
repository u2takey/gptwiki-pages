# cgroups 
## chatgpt 
Cgroups, short for Control groups, is a Linux kernel feature that enables the operating system to limit, control, and monitor the resource usage of processes or groups of processes. The cgroup feature was introduced in Linux kernel version 2.6.24 and has since been improved and enhanced to offer a wide range of resource management capabilities.

Cgroups allow the system administrator to do the following:

1. Control CPU, memory, and I/O bandwidth usage of processes or groups of processes.
2. Limit the maximum amount of memory that a process or a group of processes can use.
3. Set CPU share for processes, i.e., allocate CPU resources according to a predefined ratio or priority.
4. Prioritize disk bandwidth usage of processes, i.e., allocate disk I/O bandwidth to different groups of processes based on their priorities.
5. Monitor the usage of system resources by processes or groups of processes.

The cgroups command is used to create and manage cgroups. The syntax of the cgroup command is as follows:

`cgroup <options> {create | delete | move | set | get | attach | release} <cgroup>`

Here are the options:

1. `-h, --help`: Display the help message and exit.
2. `-V, --version`: Display the version information and exit.
3. `-g <subsys>, --subsys=<subsys>`: Specify the subsystem to use. Multiple subsystems can be specified using a comma-separated list.
4. `-a, --all`: Display information for all cgroups.
5. `-r, --recursive`: Perform the operation recursively on all child cgroups.
6. `-u <uid>, --uid=<uid>`: Set the UID of the new cgroup.
7. `-k, --kill`: Send a SIGKILL signal to all processes in the cgroup.
8. `-f, --force`: Perform the operation forcefully.
9. `<cgroup>`: The name of the cgroup.

Here are the commands and their descriptions:

1. `create`: Create a new cgroup.
2. `delete`: Delete an existing cgroup.
3. `move`: Move a cgroup to another parent cgroup.
4. `set`: Set the cgroup parameters.
5. `get`: Get the cgroup parameters.
6. `attach`: Attach a process to a cgroup.
7. `release`: Release a process from a cgroup.

To create a new cgroup, use the following command:

`sudo cgcreate -g <subsystem>:<cgroup>`

For example, to create a new cgroup named "mygroup" under the CPU subsystem, use the following command:

`sudo cgcreate -g cpu:mygroup`

To set the CPU share for a cgroup, use the following command:

`sudo cgset -r cpu.shares=<value> <cgroup>`

For example, to set the CPU share for the "mygroup" cgroup to 512, use the following command:

`sudo cgset -r cpu.shares=512 mygroup`

To attach a process to a cgroup, use the following command:

`sudo cgclassify -g <subsystem>:<cgroup> <pid>`

For example, to attach a process with PID 1234 to the "mygroup" cgroup, use the following command:

`sudo cgclassify -g cpu:mygroup 1234` 

## tldr 
 
> Cgroups aka control groups is a Linux kernel feature for limiting, measuring, and controlling resource usage by processes.
> Cgroups however is not a command, but rather a collection of commands, see the relevant pages below.
> More information: <https://www.kernel.org/doc/Documentation/cgroup-v2.txt>.

- Show the tldr page for `cgclassify`:

`tldr cgclassify`

- Show the tldr page for `cgcreate`:

`tldr cgcreate`

- Show the tldr page for `cgexec`:

`tldr cgexec`
