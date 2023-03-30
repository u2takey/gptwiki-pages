# inxi 
## chatgpt 
Inxi is a Linux command-line tool used to display relevant information about the system hardware, software, and user environment. It can be used to get information about the system's CPU, GPU, RAM, storage, network, kernel, and other system-related details.

The inxi command can be run with different options to display specific types of information. Here are some commonly used options:

- -C or --cpu: displays CPU information
- -G or --graphics: displays graphics card information
- -m or --memory: displays RAM information
- -d or --drives: displays information about storage devices
- -N or --network: displays network information
- -v or --version: displays the inxi version

By default, running the inxi command without any options will display a summary of system information, including the Linux distribution, kernel version, CPU model, RAM amount, and uptime.

Overall, the inxi command is a useful tool for quickly getting an overview of your Linux system configuration, and it can help you diagnose hardware-related issues or verify software compatibility requirements. 

## tldr 
 
> Print a summary of system information and resources for debugging purposes.
> More information: <https://manned.org/inxi>.

- Print a summary of CPU, memory, hard drive and kernel information:

`inxi`

- Print a full description of CPU, memory, disk, network and process information:

`inxi -Fz`

- Print information about the distribution's repository:

`inxi -r`
