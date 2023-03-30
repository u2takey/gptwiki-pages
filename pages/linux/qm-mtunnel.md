# qm mtunnel 
## chatgpt 
As an AI language model, I do not have a specific context of where this command is being used. However, based on my understanding:

The 'qm mtunnel' command, if using QM or QEMU-KVM virtualization systems, is used to create a macvtap tunnel for a virtual network interface. This command is typically used to allow virtual machines on the same host to communicate with each other through a dedicated virtual network, isolated from the host's physical network.

A macvtap interface is a variation of a tap interface (which simply duplicates all traffic from a physical interface to the virtual interface of a virtual machine), but instead duplicates only one virtual interface specifically created for each virtual machine, thus enabling them to communicate with each other privately.

The 'qm mtunnel' command can be executed in a terminal or command prompt, but before executing this command, you must specify the virtual machine's ID or name to assign the macvtap interface. Also, this command typically requires root privileges, so you need to execute it with 'sudo'. 

## tldr 
 
> Used by `qmigrate`.
> It should not be invoked manually.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Command used by `qmigrate` during data migration from a VM to another host:

`qm mtunnel`
