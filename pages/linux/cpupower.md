# cpupower 
## chatgpt 
cpupower is a command-line utility in Linux used to manage the CPU frequency and power management settings of the system. It is used to monitor and manage the power-saving features of the CPU, such as reducing the CPU frequency, voltage and disabling C-states. 

The cpupower command has several subcommands that perform various tasks related to CPU power management. Here are some of the commonly used subcommands of cpupower:

1. frequency-info: This subcommand is used to view the current CPU frequency and available CPUs.

2. frequency-set: This subcommand is used to set the CPU frequency of the system.

3. idle-info: This subcommand is used to view the current idle state of the CPU.

4. idle-set: This subcommand is used to set the idle mode of the CPU.

5. set: This subcommand is used to enable or disable specific power-saving features of the CPU.

Overall, the cpupower command is useful for monitoring and configuring CPU power management settings in the Linux system. It can help to conserve energy, reduce noise, and increase the lifespan of your CPU. 

## tldr 
 
> Tools regarding CPU power and tuning options.
> This command is available as part of the `cpupower` package, or as part of `kernel-tools` on Fedora.
> More information: <https://manned.org/cpupower>.

- List CPUs:

`sudo cpupower --cpu {{all}} info`

- Print information about all cores:

`sudo cpupower --cpu {{all}} info`

- Set all CPUs to a power-saving frequency governor:

`sudo cpupower --cpu {{all}} frequency-set --governor {{powersave}}`

- Print CPU 0's available frequency [g]overnors:

`sudo cpupower --cpu {{0}} frequency-info g | grep "analyzing\|governors"`

- Print CPU 4's frequency from the hardware, in a human-readable format:

`sudo cpupower --cpu {{4}} frequency-info --hwfreq --human`
