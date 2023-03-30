# qm shutdown 
## chatgpt 
The command "qm shutdown" is a command used in the Proxmox Virtual Environment (PVE) environment to shut down a virtual machine (VM). 

When you run the "qm shutdown" command, It sends a shutdown signal to the virtual machine, prompting it to perform a graceful shutdown of the operating system running within the VM. This is similar to shutting down a physical computer by clicking on the "shut down" button, instead of just unplugging it or pushing the power button.

The "qm" part of the command stands for "Qemu Manager", which is a graphical user interface software used for managing virtual machines in PVE. The "shutdown" part of the command is used to specify the desired action, which is to shut down a VM.

It is important to note that before using the "qm shutdown" command, you should save any unsaved work on the VM's operating system and close any open applications, in order to prevent data loss or corruption. Additionally, it is recommended to stop any services that may be running within the VM before issuing the shutdown command. 

Overall, the "qm shutdown" command is a useful tool for managing virtual machines in PVE and ensuring that they are shut down safely and effectively. 

## tldr 
 
> Shutdown a virtual machine on QEMU/KVM Virtual Machine Manager.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Shutdown a virtual machine:

`qm shutdown {{VM_ID}}`

- Shutdown a virtual machine after wait for at most 10 seconds:

`qm shutdown --timeout {{10}} {{VM_ID}}`

- Shutdown a virtual machine and do not deactivate storage volumes:

`qm shutdown --keepActive {{true}} {{VM_ID}}`

- Shutdown a virtual machine and skip lock (only root can use this option):

`qm shutdown --skiplock {{true}} {{VM_ID}}`

- Stop and shutdown a virtual machine:

`qm shutdown --forceStop {{true}} {{VM_ID}}`
