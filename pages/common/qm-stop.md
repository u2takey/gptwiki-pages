# qm stop 
## chatgpt 
The command "qm stop" is used in Proxmox Virtual Environment (PVE) to stop a running virtual machine (VM). 

When a VM is running, its state is considered as "up", which means the VM is actively running and consuming system resources. To stop the VM, it is required to change its state to "down", which can be done by executing the "qm stop" command. 

This command will gracefully initiate the shutdown process of the VM, which will allow it to save its data and settings before shutting down. Once the VM is shut down, its state will be changed to "stopped" in the PVE. 

It is worth noting that this command will not remove the VM, but only stop it. To remove the VM completely, another command, such as "qm destroy", will be required. 

Overall, the "qm stop" command is an essential tool in managing the virtual machines in PVE, allowing users to gracefully stop a running VM and change its state as required. 

## tldr 
 
> Stop a virtual machine.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Stop a virtual machine immediately:

`qm stop {{VM_ID}}`

- Stop a virtual machine and wait for at most 10 seconds:

`qm stop --timeout {{10}} {{VM_ID}}`

- Stop a virtual machine and skip lock (only root can use this option):

`qm stop --skiplock {{true}} {{VM_ID}}`

- Stop a virtual machine and don't deactivate storage volumes:

`qm stop --keepActive {{true}} {{VM_ID}}`
