# qm reset 
## chatgpt 
The "qm reset" command is a virtual machine management command used in Proxmox Virtual Environment (PVE). The command is used to reset a virtual machine (VM) to its original state by forcing a power-off and then restarting it. 

The "qm" part of the command refers to the "Qemu Manager" tool in PVE, which is used to manage virtual machines. The "reset" option refers to the specific task that needs to be performed on the VM. 

When you execute the "qm reset" command, it will power off the specified virtual machine immediately, which will stop all the running processes inside the VM. Once the VM is powered off, it will then restart it as if it is starting from scratch, wiping out any changes that may have been made since the last time the VM was started. 

This command can be used to fix issues with a virtual machine that has become unresponsive or unstable. However, it should be used with caution as it will result in the loss of any unsaved data or changes made inside the VM since the last backup or snapshot. 

## tldr 
 
> Reset a virtual machine on QEMU/KVM Virtual Machine Manager.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Reset a virtual machine:

`qm reset {{vm_id}}`

- Reset a virtual machine and skip lock (only root can use this option):

`qm reset --skiplock {{true}} {{vm_id}}`
