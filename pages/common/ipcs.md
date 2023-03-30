# ipcs 
## chatgpt 
The `ipcs` command is a Linux/Unix command that stands for "interprocess communication (IPC) facilities status". It is used to display information about system resources that are used for interprocess communication, such as message queues, shared memory segments, and semaphores. 

The `ipcs` command displays information in three categories: 

1. Message Queues: This section contains information about message queues such as the ID, owner user ID, group ID, permissions, number of messages in queue, max size of messages, etc. 

2. Shared Memory: This section displays information about shared memory segments such as the ID, owner user ID, group ID, permissions, size of shared memory segments, etc. 

3. Semaphores: This section displays information about semaphores such as ID, owner user ID, group ID, permission, semaphore array value, lock status, etc.

The `ipcs` command does not modify any system resources, it just displays their current status. It can be useful for system administrators to monitor system resource usage and diagnose issues related to interprocess communication. 

## tldr 
 
> Display information about resources used in IPC (Inter-process Communication).
> More information: <https://manned.org/ipcs>.

- Specific information about the Message Queue which has the ID 32768:

`ipcs -qi 32768`

- General information about all the IPC:

`ipcs -a`
