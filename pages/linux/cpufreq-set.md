# cpufreq-set 
## chatgpt 
cpufreq-set is a command used in Linux operating systems to manipulate CPU frequency scaling settings. It is typically used to adjust the clock speed of a processor in order to optimize power usage, reduce energy consumption, and improve performance. 

The command allows you to set various parameters related to CPU frequency scaling, such as:

- Minimum and maximum frequency: The minimum frequency refers to the lowest clock speed the processor can operate at, while the maximum frequency is the highest clock speed it can reach.
- Scaling governor: The scaling governor is a kernel module that determines how the CPU frequency is adjusted in response to different workloads. The available governors include "powersave", "performance", "ondemand", and "conservative".
- CPU number: The command can be run on a specific CPU core, allowing you to adjust the frequency of a particular processor in a multi-core system.
- Frequency stepping: Some processors support a feature called frequency stepping, which allows them to change frequency in small increments. The cpufreq-set command can be used to enable or disable this feature.

To use the cpufreq-set command, you need to have root access or run it as a superuser. 

The syntax for the command is:

cpufreq-set [options]

Here are some examples of how to use the command:

To set the minimum and maximum frequency of the CPU to 800 MHz and 1.2 GHz respectively, you can run:

sudo cpufreq-set -c 0 -f 800MHz -u 1.2GHz

Here, -c 0 specifies that the changes should be applied to the first CPU core, -f 800MHz sets the minimum CPU frequency to 800 MHz, and -u 1.2GHz sets the maximum CPU frequency to 1.2 GHz.

To set the scaling governor to "ondemand", run:

sudo cpufreq-set -c 0 -g ondemand

Here, -g ondemand sets the scaling governor to "ondemand", which adjusts the CPU frequency based on the workload.

Overall, the cpufreq-set command is a powerful tool for system administrators and power users who want to optimize their system's efficiency and performance. 

## tldr 
 
> A tool to modify CPU frequency settings.
> The frequency value should range between the output of command `cpufreq-info -l`.
> More information: <https://manned.org/cpufreq-set>.

- Set the CPU frequency policy of CPU 1 to "userspace":

`sudo cpufreq-set -c {{1}} -g {{userspace}}`

- Set the current minimum CPU frequency of CPU 1:

`sudo cpufreq-set -c {{1}} --min {{min_frequency}}`

- Set the current maximum CPU frequency of CPU 1:

`sudo cpufreq-set -c {{1}} --max {{max_frequency}}`

- Set the current work frequency of CPU 1:

`sudo cpufreq-set -c {{1}} -f {{work_frequency}}`
