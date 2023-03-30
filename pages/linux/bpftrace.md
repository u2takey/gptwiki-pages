# bpftrace 
## chatgpt 
Bpftrace is a dynamic tracing tool for Linux that is based on extended Berkeley Packet Filter (eBPF) technology. It allows system engineers and developers to trace and analyze different aspects of their Linux systems, including kernel function calls, system calls, driver behavior, and network activity.

Bpftrace scripts are written in a high-level language that is easy to use and understand. They are compiled into eBPF bytecode and executed in the kernel. Bpftrace provides a range of built-in functions and variables that can be used in the scripts, as well as support for custom functions and user-defined tracing events.

With bpftrace, the system administrator or developer can monitor and analyze various system events in real-time without incurring significant performance overhead. This includes detecting performance bottlenecks, security threats, and unexpected behavior.

Some common use cases for bpftrace include system resource profiling, network traffic analysis, memory usage tracking, process monitoring, and system call tracing. It is a powerful and versatile tool that can be used for a wide variety of tasks related to system performance and security. 

## tldr 
 
> High-level tracing language for Linux eBPF.
> More information: <https://github.com/iovisor/bpftrace>.

- Display bpftrace version:

`bpftrace -V`

- List all available probes:

`sudo bpftrace -l`

- Run a one-liner program (e.g. syscall count by program):

`sudo bpftrace -e '{{tracepoint:raw_syscalls:sys_enter { @[comm] = count(); }}}'`

- Run a program from a file:

`sudo bpftrace {{path/to/file}}`

- Trace a program by PID:

`sudo bpftrace -e '{{tracepoint:raw_syscalls:sys_enter /pid == 123/ { @[comm] = count(); }}}'`

- Do a dry run and display the output in eBPF format:

`sudo bpftrace -d -e '{{one_line_program}}'`
