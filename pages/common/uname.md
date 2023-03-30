# uname 
## chatgpt 
The command "uname"stands for "Unix Name" and is a built-in command in most Unix-based operating systems like Linux and macOS. It is used to display system information about the operating system running on the current machine.

Here are the options and parameters that can be used with the "uname" command:

- "a" or "–all" - Displays all the information about the system.

- "s" or "–kernel-name" - Displays the kernel name of the system.

- "n" or "–nodename" - Displays the name of the network node.

- "r" or "–kernel-release" - Displays the release number of the kernel.

- "v" or "–kernel-version" - Displays the version number of the kernel.

- "m" or "–machine" - Displays the name of the machine.

- "p" or "–processor" - Displays the processor type.

- "i" or "–hardware-platform" - Displays the hardware platform.

- "o" or "–operating-system" - Displays the name of the operating system.

For example, if you want to display all the information about the system, type "uname -a" and press Enter. If you want to know the kernel name of your system, use "uname -s". Similarly, enter "uname -n" to know the network name, "uname -r" to know the kernel release, "uname -v" to know the kernel version, "uname -m" to know the machine name, "uname -p" to know the processor type, and "uname -o" to know the operating system name. 

## tldr 
 
> Print details about the current machine and the operating system running on it.
> See also `lsb_release`.
> More information: <https://www.gnu.org/software/coreutils/uname>.

- Print kernel name:

`uname`

- Print system architecture and processor information:

`uname --machine --processor`

- Print kernel name, kernel release and kernel version:

`uname --kernel-name --kernel-release --kernel-version`

- Print system hostname:

`uname --nodename`

- Print all available system information:

`uname --all`
