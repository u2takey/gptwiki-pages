# cpuid 
## chatgpt 
The "cpuid" command is used to display information about the CPU (Central Processing Unit) of a computer system. It is a system utility command that is executed on the command line or terminal window. On executing the "cpuid" command, it accesses the CPUID instruction of the processor to retrieve the CPU identification and feature information. 

The CPUID instruction is a processor instruction that allows the CPU to identify itself and retrieve information about its features and capabilities. It is supported by all modern processors and is used by the operating system to determine the type and features of the CPU. 

When executed, the "cpuid" command displays various information about the CPU of the system, including the manufacturer name, model name, stepping, family, and model numbers. It also displays feature flags that indicate the various capabilities of the CPU, such as support for virtualization, extended instruction sets, and CPU speed. 

Overall, the "cpuid" command is a useful tool for system administrators, developers, and users who need to identify the type and features of the CPU in a computer system. 

## tldr 
 
> Display detailed information about all CPUs.
> More information: <http://etallen.com/cpuid.html>.

- Display information for all CPUs:

`cpuid`

- Display information only for the current CPU:

`cpuid -1`

- Display raw hex information with no decoding:

`cpuid -r`
