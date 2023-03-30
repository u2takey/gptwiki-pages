# pixiecore 
## chatgpt 
As an AI language model, I cannot perform any commands on a computer, but I can explain what the "pixiecore" command is and what it does.

Pixiecore is a lightweight open-source network boot firmware designed for embedded systems and cloud services. It is mainly used to boot operating system images over the network, which can be useful for systems that don’t have any internal storage or where the storage is not suitable for booting an OS.

This software can be used as a replacement for more complicated boot firmware like GRUB or UEFI. It is written in Golang and can be run on a variety of architectures, including x86, ARM, and PowerPC.

Pixiecore supports multiple protocols like PXE, HTTP, and TFTP to perform network booting. It also has features like dynamic network configuration, which enables the system to obtain an IP address and other configuration parameters automatically from a DHCP server.

In summary, the "pixiecore" command is a tool used to boot operating system images over a network in embedded systems and cloud services, and it is written in Golang. 

## tldr 
 
> Tool to manage the network booting of machines.
> More information: <https://github.com/danderson/netboot/tree/master/pixiecore>.

- Start a PXE boot server which provides a `netboot.xyz` boot image:

`pixiecore {{quick}} xyz --dhcp-no-bind`

- Start a new PXE boot server which provides an Ubuntu boot image:

`pixiecore {{quick}} ubuntu --dhcp-no-bind`

- Get a list of all available boot images for quick mode:

`pixiecore quick --help`
