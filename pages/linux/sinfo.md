# sinfo 
## chatgpt 
The sinfo command is used in high-performance computing (HPC) systems to display information about the system's resources and the current state of the cluster. Here is an overview of what the sinfo command displays:

- Node information: The sinfo command shows the name of each node in the cluster along with its current state (e.g. idle, down, drained, etc.), the number of CPUs, and the amount of memory and disk space available.

- Partition information: If the HPC system is divided into partitions (also called "queues"), the sinfo command shows the name of each partition along with the same details as for the nodes.

- Scheduling policy: The sinfo command displays the current scheduling policy for the system, which determines how jobs are queued and run on the cluster.

- Time and load averages: Finally, the sinfo command shows the current time on the system and the average load across all nodes, which provides an indication of how busy the cluster is.

Overall, the sinfo command is a useful tool for system administrators, HPC users, and software developers to get a quick overview of the system's resources and status, which can help them plan their workloads, optimize job scheduling, and troubleshoot any issues that may arise. 

## tldr 
 
> View information about Slurm nodes and partitions.
> See also `squeue` and `sbatch`, which are also part of the Slurm workload manager.
> More information: <https://slurm.schedmd.com/sinfo.html>.

- Show a quick summary overview of the cluster:

`sinfo --summarize`

- View the detailed status of all partitions across the entire cluster:

`sinfo`

- View the detailed status of a specific partition:

`sinfo --partition {{partition_name}}`

- View information about idle nodes:

`sinfo --states {{idle}}`

- Summarise dead nodes:

`sinfo --dead`

- List dead nodes and the reasons why:

`sinfo --list-reasons`
