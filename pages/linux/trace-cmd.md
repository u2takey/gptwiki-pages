# trace-cmd 
## chatgpt 
The `trace-cmd` command is a tool used for tracing system events and performance metrics on a Linux system. It is a command-line utility that allows users to monitor, analyze, and debug various system activities. The primary objective of `trace-cmd` is to capture low-level events in the system such as system calls, interrupts, file I/O, network I/O, and other kernel activities. 

Here's a description of some of the key options you can use with `trace-cmd`:

- `start`: This option starts the tracing process. This command needs to be followed by a command that is to be traced. For example, `trace-cmd start -p function_name` could be used to trace a specific function in a program.
- `list`: This option lists all the available events that can be traced on the system. The `list` command provides a list of event plugins available in the system. These plugins could be activated to trace any specific trace event. For example, `trace-cmd list -e cpu_frequency` could be used to list all the available tracing events related to CPU frequency.
- `stop`: This option stops the tracing process. It is used to finish the tracing process and generate the log files. 
- `extract`: This option is used to extract trace data from a saved capture file. By using the `extract` command, users can pull out specific events or ranges of events from a trace file. This works on saved trace data files which are generated while tracing the system.
- `report`: This option is used to generate a report based on the captured trace data. The `report` command displays graphs and statistics for the collected events. This command is helpful to analyze the performance of a system.

In summary, the `trace-cmd` command is a powerful tracing tool that helps in debugging problems related to various system events and activities. It is widely used by developers, system administrators, and performance engineers to optimize system performance, and to diagnose performance issues. 

## tldr 
 
> Utility to interact with the Ftrace Linux kernel internal tracer.
> This utility only runs as root.
> More information: <https://manned.org/trace-cmd>.

- Display the status of tracing system:

`trace-cmd stat`

- List available tracers:

`trace-cmd list -t`

- Start tracing with a specific plugin:

`trace-cmd start -p {{timerlat|osnoise|hwlat|blk|mmiotrace|function_graph|wakeup_dl|wakeup_rt|wakeup|function|nop}}`

- View the trace output:

`trace-cmd show`

- Stop the tracing but retain the buffers:

`trace-cmd stop`

- Clear the trace buffers:

`trace-cmd clear`

- Clear the trace buffers and stop tracing:

`trace-cmd reset`
