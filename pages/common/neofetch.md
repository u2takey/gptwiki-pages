# neofetch 
## chatgpt 
neofetch is a command-line utility that displays system information, including OS version, kernel version, CPU and GPU information, memory usage, disk usage, and more.

When the neofetch command is executed in a terminal, it gathers and displays various details about the user's computer system. These details include:

- The operating system and distribution name
- The system hostname
- The kernel version number
- The CPU model, speed, and usage percentage
- The GPU model and memory usage
- The amount of RAM and swap space used
- Information about the installed storage devices, including the file system type and amount of used and available space
- The current desktop environment or window manager

The output of the neofetch command is highly customizable and can be modified to include or exclude specific details or to display certain elements in the system logo, such as the CPU or GPU logo.

Overall, neofetch is a useful command for quickly displaying essential system information in a terminal, which can be helpful in understanding the current state and performance of the user's computer system. 

## tldr 
 
> CLI tool to display information about your operating system, software and hardware.
> More information: <https://github.com/dylanaraps/neofetch>.

- Return the default config, and create it if it's the first time the program runs:

`neofetch`

- Trigger an info line from appearing in the output, where 'infoname' is the function name in the config file, e.g. memory:

`neofetch --{{enable|disable}} {{infoname}}`

- Hide/Show OS architecture:

`neofetch --os_arch {{on|off}}`

- Enable/Disable CPU brand in output:

`neofetch --cpu_brand {{on|off}}`
