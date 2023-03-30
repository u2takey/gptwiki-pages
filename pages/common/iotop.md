# iotop 
## chatgpt 
The iotop command is a Linux system monitoring tool that allows users to observe input/output (I/O) usage by processes in real-time. With iotop, users can identify which processes are using the most I/O resources and troubleshoot problematic processes that may be causing system slowdowns.

When you run the iotop command, you will typically see a list of processes that are currently using I/O resources, along with information about how much data they are reading and/or writing. The output from iotop is updated periodically, so you can see changes to I/O usage over time.

Some commonly used options with iotop include the -a flag, which shows all processes (including those that aren't doing I/O), the -u flag, which lets you filter by user, and the -P flag, which lets you filter by process name or ID.

Overall, iotop is a useful tool for system administrators and other Linux users who need to monitor I/O usage and pinpoint resource-intensive processes. 

## tldr 
 
> Display a table of current I/O usage by processes or threads.
> More information: <https://manned.org/iotop>.

- Start top-like I/O monitor:

`sudo iotop`

- Show only processes or threads actually doing I/O:

`sudo iotop --only`

- Show I/O usage in non-interactive mode:

`sudo iotop --batch`

- Show only I/O usage of processes (default is to show all threads):

`sudo iotop --processes`

- Show I/O usage of given PID(s):

`sudo iotop --pid={{PID}}`

- Show I/O usage of a given user:

`sudo iotop --user={{user}}`

- Show accumulated I/O instead of bandwidth:

`sudo iotop --accumulated`
