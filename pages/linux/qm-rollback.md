# qm rollback 
## chatgpt 
The "qm rollback" command is used in the Proxmox Virtual Environment (PVE) to rollback a virtual machine (VM) to a previously saved snapshot. When a snapshot is taken for a VM, it captures the VM's state at a particular point in time, including the disk state, memory state, and virtual hardware configuration.

When you issue the "qm rollback" command, it searches for the snapshots that were taken for that particular VM and displays them, along with their respective names and creation timestamps. You can then select the snapshot you want to revert to and proceed with the rollback process. When you rollback a VM to a previous snapshot, all changes made to the VM after the snapshot was taken will be discarded.

The "qm rollback" command is useful when you encounter issues or errors after making significant changes to a VM, as it enables you to easily revert back to a known working state. However, it's important to note that rolling back a VM to a snapshot could result in data loss, so it's recommended to take a backup of the VM before proceeding with the rollback. 

## tldr 
 
> Rollback the VM state to a specified snapshot.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Rollback the state of a specific VM to a specified snapshot:

`qm rollback {{vm_id}} {{snap_name}}`
