# numactl 
## chatgpt 
The `numactl` command is a Linux utility that allows you to control and monitor the NUMA (Non-Uniform Memory Access) behavior of processes and memory allocation. NUMA is a hardware architecture where different regions of memory have different latencies and bandwidths depending on the processor that accesses them. The `numactl` command helps to optimize performance by providing better control over how memory and CPUs are allocated in systems with multiple CPUs and memory controllers.

Here are some common options and use cases for `numactl`:

- `-H`: Displays information about the NUMA topology of the system, including the number of nodes, processors, and memory. This can help you understand how memory and CPUs are physically connected and how the system will allocate resources.
- `-l`: Binds a process to a specific set of CPUs or nodes. This can help you control where the process runs and where it allocates memory, which can affect performance.
- `-p`: Binds a process to its local memory node. This can help improve performance by reducing the amount of time it takes for a processor to access memory.
- `-m`: Specifies the memory policy for a process or command. This can help control how memory is allocated and accessed. For example, you can use this option to prioritize memory access to certain nodes or to balance memory usage across nodes.
- `-N`: Specifies the node(s) on which a process or command should be run. This can help optimize performance by keeping the process closer to its memory and reducing memory access latency.

Overall, `numactl` is a powerful tool for optimizing performance in systems with NUMA architecture. By using the options and commands available in `numactl`, you can gain more control over the allocation of memory and CPUs and improve overall system performance. 

## tldr 
 
> Control NUMA policy for processes or shared memory.
> More information: <https://man7.org/linux/man-pages/man8/numactl.8.html>.

- Run a command on node 0 with memory allocated on node 0 and 1:

`numactl --cpunodebind={{0}} --membind={{0,1}} -- {{command}} {{command_arguments}}`

- Run a command on CPUs (cores) 0-4 and 8-12 of the current cpuset:

`numactl --physcpubind={{+0-4,8-12}} -- {{command}} {{command_arguments}}`

- Run a command with its memory interleaved on all CPUs:

`numactl --interleave={{all}} -- {{command}} {{command_arguments}}`
