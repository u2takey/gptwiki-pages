# pmap 
## chatgpt 
The pmap command is a command-line utility available in Unix-like operating systems that displays the memory map of a process or set of processes. The memory map is a description of the different memory segments a process is using, and includes information such as memory addresses, permissions, and flags.

The syntax for the pmap command is as follows:

```
pmap [options] [pid | program]
```

- `options`: this can include any combination of the following options:
  - `-d`: Display the memory map in decimal format.
  - `-x`: Display the memory map in hexadecimal format.
  - `-q`: Quiet mode. Only display the memory addresses and permissions.
  - `-x`: Display the memory map in hexadecimal format.
  - `-XX`: Display the hexadecimal dump of the process image.
  - `-C`: Display the shared libraries that the process is using.
  - `-p`: Display the memory map of a particular process with the given PID number.
  
- `pid | program`: This is an optional argument that specifies the PID of the process, or a program name whose memory map is to be displayed. If no argument is specified, the memory map of the shell process is displayed by default.

When used, the pmap command displays the memory map of the specified process or program in the specified format, as well as additional information like the total size of the process, the amount of memory used, and the libraries it is linked against. This information can be used by developers and system administrators to optimize the memory usage of various programs and processes, as well as to identify potential memory leaks, security issues, and other performance issues. 

## tldr 
 
> Report memory map of a process or processes.
> More information: <https://manned.org/pmap>.

- Print memory map for a specific process id (PID):

`pmap {{pid}}`

- Show the extended format:

`pmap --extended {{pid}}`

- Show the device format:

`pmap --device {{pid}}`

- Limit results to a memory address range specified by `low` and `high`:

`pmap --range {{low}},{{high}}`

- Print memory maps for multiple processes:

`pmap {{pid1 pid2 ...}}`
