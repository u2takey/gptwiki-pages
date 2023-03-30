# cpufreq-info 
## chatgpt 
The `cpufreq-info` command is used to display information about the CPU frequency scaling. This command is typically used on Linux operating systems to get information about the CPU frequency scaling policy for the processor in use. 

The command provides detailed information about the current CPU frequency scaling governor and the available governors on the system. It also provides information about the current CPU frequency, both in MHz and as a percentage of the maximum frequency.

The `cpufreq-info` command may allow the user to determine if the processor is running in a low-power mode, or if it is capable of boosting its clock frequency automatically to handle high-performance loads.

This command is useful for system administrators and power users who want to monitor and optimize the performance of their systems, like managing power usage, heat and noise reduction, and other related issues regarding the processor. 

## tldr 
 
> A tool to show CPU frequency information.
> More information: <https://manned.org/cpufreq-info>.

- Show CPU frequency information for all CPUs:

`cpufreq-info`

- Show CPU frequency information for the specified CPU:

`cpufreq-info -c {{cpu_number}}`

- Show the allowed minimum and maximum CPU frequency:

`cpufreq-info -l`

- Show the current minimum and maximum CPU frequency and policy in table format:

`cpufreq-info -o`

- Show available CPU frequency policies:

`cpufreq-info -g`

- Show current CPU work frequency in a human-readable format, according to the cpufreq kernel module:

`cpufreq-info -f -m`

- Show current CPU work frequency in a human-readable format, by reading it from hardware (only available to root):

`sudo cpufreq-info -w -m`
