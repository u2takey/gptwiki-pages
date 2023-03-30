# qm guest passwd 
## chatgpt 
The command "qm guest passwd" is used in the context of the Proxmox Virtual Environment (PVE), which is an open-source virtualization management platform. Here the command qm stands for "QEMU machine", which is used to manage and configure virtual machines.

The qm guest passwd command is used to change the password of a guest virtual machine running in a PVE environment. This command is used to change the login password of the guest virtual machine, which is used to access the system. 

Here is the syntax of the qm guest passwd command:

qm guest passwd <vmid>

The "vmid" refers to the ID of the virtual machine for which we want to change the password. After executing this command, PVE will prompt the user to enter a new password. Once the new password is entered and confirmed, it will be updated on the guest virtual machine.

It's important to note that the qm guest passwd command requires root privileges for execution. This command can also be used with other options such as --user to specify a specific user whose password needs to be changed. 

## tldr 
 
> Set the password for a specific user on QEMU/KVM Virtual Machine Manager.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Set a password for a specific user in a virtual machine interactively:

`qm guest passwd {{vm_id}} {{username}}`

- Set an already hashed password for a specific user in a virtual machine interactively:

`qm guest passwd {{vm_id}} {{username}} --crypted 1`
