# nproc 
## chatgpt 
The `nproc` command is a simple Linux command that is used to display the number of processing units (or CPUs) available on the current system.

When the `nproc` command is executed, it reads the `/proc/cpuinfo` file, which contains information about the system's CPUs such as the number of cores, sockets, threads, and other attributes.

The `nproc` command then uses this information to determine the number of processing units available on the system and displays it on the terminal.

So, for example, if a system has 4 CPU cores and supports hyper-threading, the `nproc` command will display 8 as the output value.

The `nproc` command is useful in scripts and applications that need to optimize resource allocation, workload distribution, or multi-processing tasks. It is also used in system administration and troubleshooting tasks to check the status and configuration of the system's CPUs. 

## tldr 
 
> Print the number of processing units (normally CPUs) available.
> More information: <https://www.gnu.org/software/coreutils/nproc>.

- Display the number of available processing units:

`nproc`

- Display the number of installed processing units, including any inactive ones:

`nproc --all`

- If possible, subtract a given number of units from the returned value:

`nproc --ignore {{count}}`
