# qm destroy 
## chatgpt 
The command "qm destroy" is used in Proxmox Virtual Environment (PVE) to delete or remove a virtual machine (VM) from the system. It permanently destroys the VM and all its associated files and settings.

The syntax of the command is:

qm destroy <vmid>

where "vmid" is the ID of the VM that you want to delete.

Before executing this command, you should make sure that the VM is not running, otherwise, it will not be possible to destroy it. You can check the status of a VM using the "qm status <vmid>" command.

When you run the "qm destroy" command, it will prompt you for confirmation before proceeding with the destruction of the VM. Once you confirm, the VM will be deleted from the system.

It is important to note that this command is irreversible and will permanently erase all data associated with the VM. Therefore, you should only use it if you are absolutely sure that you want to delete the VM.

In summary, the "qm destroy" command is used in PVE to permanently delete a virtual machine and all its data from the system. 

## tldr 
 
> Destroy a virtual machine in QEMU/KVM Virtual Machine Manager.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Destroy a specific virtual machine:

`qm destroy {{vm_id}}`

- Destroy all disks that are not explicitly referenced in a specific virtual machine's configuration:

`qm destroy {{vm_id}} --destroy-unreferenced-disks`

- Destroy a virtual machine and remove from all locations (inventory, backup jobs, high availability managers, etc.):

`qm destroy {{vm_id}} --purge`

- Destroy a specific virtual machine ignoring locks and forcing destroy:

`sudo qm destroy {{vm_id}} --skiplock`
