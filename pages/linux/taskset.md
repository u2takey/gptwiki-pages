# taskset 
## chatgpt 
Taskset is a Linux command that allows users to control the CPU affinity of running processes. CPU affinity determines which CPUs are allowed to execute a particular process, thread, or set of threads.

The basic syntax of the command is as follows:

taskset [options] [mask] [command] [arguments]

Options:
- c: CPU selection mode
- p: Attach a running process to a CPU
- q: Query current CPU affinity
- r: Set CPU affinity of a range of CPUs
- s: Set CPU affinity of a group of CPUs

Mask:
- A hexadecimal number indicating the set of CPUs where the task should be allowed to run. For example, a mask of 0x3 would allow the task to run on CPUs 0 and 1.

Command:
- The command to run with the specified CPU affinity.

Arguments:
- Any arguments to be passed to the command.

For example, the command 'taskset -c 0,2,4 ./myprogram' would execute the 'myprogram' with CPU affinity restricted to CPUs 0, 2, and 4.

Overall, taskset is a useful command for optimizing the performance of running processes by restricting them to certain CPUs, thereby reducing contention and interference between processes. 

## tldr 
 
> Get or set a process' CPU affinity or start a new process with a defined CPU affinity.
> More information: <https://manned.org/taskset>.

- Get a running process' CPU affinity by PID:

`taskset --pid --cpu-list {{pid}}`

- Set a running process' CPU affinity by PID:

`taskset --pid --cpu-list {{cpu_id}} {{pid}}`

- Start a new process with affinity for a single CPU:

`taskset --cpu-list {{cpu_id}} {{command}}`

- Start a new process with affinity for multiple non-sequential CPUs:

`taskset --cpu-list {{cpu_id_1}},{{cpu_id_2}},{{cpu_id_3}}`

- Start a new process with affinity for CPUs 1 through 4:

`taskset --cpu-list {{cpu_id_1}}-{{cpu_id_4}}`
