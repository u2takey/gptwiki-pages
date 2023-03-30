# ulimit 
## chatgpt 
The 'ulimit' command in Linux is used to set, change and display the resource limits for a user or a group of users. The resource limits or restrictions that can be set using the 'ulimit' command include:

- CPU time limit (in seconds)
- Maximum size of a file (in blocks)
- Maximum number of open files
- Maximum size of virtual memory
- Maximum size of a core file (in blocks)
- Maximum size of a process' data segment

The 'ulimit' command has the following syntax:

```
ulimit [OPTION] [value]
```

Where 'OPTION' can be one of the following:

- '-a' - displays all the current resource limits of the user
- '-c' - the maximum size of a core file
- '-d' - the maximum size of the data segment of a process
- '-e' - the maximum scheduling priority
- '-f' - the maximum size of a file that can be created by the user
- '-i' - the maximum number of processes that can be created by the user
- '-l' - the maximum size of a process' locked memory
- '-m' - the maximum size of virtual memory available to a process
- '-n' - the maximum number of open file descriptors a process can have
- '-p' - the pipe size in bytes
- '-q' - the maximum number of bytes in a message queue
- '-r' - the maximum real-time scheduling priority
- '-s' - the maximum size of a stack segment of a process
- '-t' - the maximum amount of CPU time a process can use
- '-u' - the maximum number of user processes

The 'value' parameter is used to set a new value for the specified resource limit.

To display the current value of a resource limit, you can use the 'ulimit' command with the appropriate option, for example:

```
ulimit -a
```

This will display all the current resource limits for the user.

To set a new value for a resource limit, you can use the same command with the appropriate option and value, for example:

```
ulimit -n 10000
```

This will set the maximum number of open file descriptors to 10000.

Please note that the resource limits set using the 'ulimit' command apply only to the current shell session and its child processes. They do not affect other users or the system as a whole. 

## tldr 
 
> Get and set user limits.
> More information: <https://manned.org/ulimit>.

- Get the properties of all the user limits:

`ulimit -a`

- Get hard limit for the number of simultaneously opened files:

`ulimit -H -n`

- Get soft limit for the number of simultaneously opened files:

`ulimit -S -n`

- Set max per-user process limit:

`ulimit -u 30`
