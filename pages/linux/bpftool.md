# bpftool 
## chatgpt 
The "bpftool" command is a Linux utility that allows users to interact with eBPF (extended Berkeley Packet Filter) programs in the Linux kernel. It provides a flexible and powerful interface for querying and manipulating various aspects of eBPF programs and maps.

Some of the most common features of bpftool include:

- Listing all available eBPF programs and maps in the kernel.
- Loading and unloading eBPF programs and maps.
- Querying eBPF map contents and statistics.
- Debugging eBPF programs using the "tracer" subcommand, which can be used to extract various information during program execution (such as function calls, register values, etc.).

Bpftool is a very powerful tool for developers and system administrators who need to work with eBPF programs and maps in the Linux kernel. Its comprehensive set of commands and options provide a great deal of flexibility and granularity in managing and monitoring eBPF programs and maps. 

## tldr 
 
> Tool for inspection and simple manipulation of eBPF programs and maps.
> Some subcommands such as `bpftool prog` have their own usage documentation.
> More information: <https://manned.org/bpftool>.

- List information about loaded `eBPF` programs:

`bpftool prog list`

- List `eBPF` program attachments in the kernel networking subsystem:

`bpftool net list`

- List all active links:

`bpftool link list`

- List all `raw_tracepoint`, `tracepoint`, `kprobe` attachments in the system:

`bpftool perf list`

- List `BPF Type Format (BTF)` data:

`bpftool btf list`

- List information about loaded maps:

`bpftool map list`

- Probe a network device "eth0" for supported `eBPF` features:

`bpftool feature probe dev {{eth0}}`

- Run commands in batch mode from a file:

`bpftool batch file {{myfile}}`
