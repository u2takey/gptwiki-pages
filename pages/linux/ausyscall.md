# ausyscall 
## chatgpt 
The "ausyscall" command is a tool provided by the Audit subsystem in Linux that serves as a system call event auditing mechanism. It allows the user to list, search and decode system call events that have been audited by the Kernel Audit framework. Each system call used by a process is audited in the kernel and the information about the system call event along with its arguments is written to the audit log. The "ausyscall" command with various arguments can be used to extract this information and decode it into a more human-readable format.

Some common uses of the "ausyscall" command are:

- Listing all the available system call numbers and their names on the system: `ausyscall -l`
- Searching the audit log for a particular system call event: `ausearch -sc <syscall_number>`
- Decoding the audit log entry for a system call event: `aureport -au -ts recent | grep <syscall_name> | ausyscall -x`

In summary, the "ausyscall" command is a useful tool for system administrators, security analysts and developers to monitor and analyze system call events and their arguments for auditing and security purposes. 

## tldr 
 
> Program that allows mapping syscall names and numbers.
> More information: <https://manned.org/ausyscall>.

- Display syscall number of a specific system call:

`ausyscall {{search_pattern}}`

- Display name of a specific system call number:

`ausyscall {{system_call_number}}`

- Display all system calls for a specific architecture:

`ausyscall {{architecture}} --dump`
