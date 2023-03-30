# kill 
## chatgpt 
The "kill" command is used in Unix-based operating systems (such as Linux, macOS, and FreeBSD) to terminate a process by sending a signal to it. The syntax for the "kill" command is as follows:

kill [signal] [process ID]

The "signal" parameter specifies which signal to send to the process. If no signal is specified, the default signal is SIGTERM (terminate). Here are some common signals used with the "kill" command:

- SIGTERM (terminate): This is the default signal sent when no signal is specified. It politely asks the process to terminate and lets it clean up any resources it has allocated before exiting.

- SIGKILL (kill): This signal immediately terminates the process without giving it a chance to clean up any resources. Use this signal as a last resort if the process is unresponsive to SIGTERM.

- SIGHUP (hang up): This signal is traditionally used to tell a process to re-read its configuration files. In some cases, it can also be used to terminate a process.

The "process ID" parameter specifies which process to terminate. You can find the process ID of a running process using the "ps" command.

In summary, the "kill" command is used to terminate a process by sending a signal to it. The signal can be specified, or the default SIGTERM signal will be used. The process ID of the target process must also be specified. 

## tldr 
 
> Sends a signal to a process, usually related to stopping the process.
> All signals except for SIGKILL and SIGSTOP can be intercepted by the process to perform a clean exit.
> More information: <https://manned.org/kill>.

- Terminate a program using the default SIGTERM (terminate) signal:

`kill {{process_id}}`

- List available signal names (to be used without the `SIG` prefix):

`kill -l`

- Terminate a background job:

`kill %{{job_id}}`

- Terminate a program using the SIGHUP (hang up) signal. Many daemons will reload instead of terminating:

`kill -{{1|HUP}} {{process_id}}`

- Terminate a program using the SIGINT (interrupt) signal. This is typically initiated by the user pressing `Ctrl + C`:

`kill -{{2|INT}} {{process_id}}`

- Signal the operating system to immediately terminate a program (which gets no chance to capture the signal):

`kill -{{9|KILL}} {{process_id}}`

- Signal the operating system to pause a program until a SIGCONT ("continue") signal is received:

`kill -{{17|STOP}} {{process_id}}`

- Send a `SIGUSR1` signal to all processes with the given GID (group id):

`kill -{{SIGUSR1}} -{{group_id}}`
