# qm reboot 
## chatgpt 
The command "qm reboot" is used to reboot a virtual machine (VM) in the Proxmox Virtual Environment (PVE) platform. 

"qm" stands for "QEMU machine" which refers to the virtual machine. The qm command is used to manage VMs in PVE. 

"reboot" indicates the action that is being performed, which is a restart of the VM. This command will shut down the VM and start it up again, effectively rebooting the entire system.

It is important to note that this command should be used with caution, as it will force any running applications on the VM to terminate, and any unsaved data will be lost. It is recommended to properly shut down the VM before using the reboot command. 

## tldr 
 
> Reboot a virtual machine by shutting it down, and starting it again after applying pending changes.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Reboot a virtual machine:

`qm reboot {{vm_id}}`

- Reboot a virtual machine after wait for at most 10 seconds:

`qm reboot --timeout {{10}} {{vm_id}}`
