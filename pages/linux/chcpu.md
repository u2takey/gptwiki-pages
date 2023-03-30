# chcpu 
## chatgpt 
The `chcpu` command is a command used in Unix-like operating systems that allows the administrator to change the settings of the system's CPU, such as adding or removing CPUs from a running system or manipulating the configuration of the system's CPU resources.

The `chcpu` command is usually reserved for system administrators who need to manage the CPU resources of a multi-CPU system, and may require root or superuser privileges to use. 

The specific syntax and functionality of the `chcpu` command may vary between different Unix-like systems, but typically the command will accept a range of arguments or options that can be used to modify the CPU settings for the system or for individual processes running on the system.

Some of the common uses of the `chcpu` command may include:

- Adding or removing CPUs from a running system 
- Setting the priority or affinity of CPUs for specific processes or threads 
- Limiting or increasing the number of CPUs available to specific processes 
- Configuring the CPU frequency, speed, or voltage of the system 
- Setting the CPU caching and prefetching settings. 

Overall, the `chcpu` command is a powerful tool for system administrators to manage and optimize the CPU resources of a Unix-like system to ensure optimal performance and stability. 

## tldr 
 
> Enable/disable a system's CPUs.
> More information: <https://manned.org/chcpu>.

- Disable CPUs via a list of CPU ID numbers:

`chcpu -d {{1,3}}`

- Enable a set of CPUs via a range of CPU ID numbers:

`chcpu -e {{1-10}}`
