# qm delsnapshot 
## chatgpt 
The "qm delsnapshot" command is used in the context of a virtualization platform called Proxmox VE (PVE), which is used for managing and consolidating multiple virtual machines (VMs) on a single server.

The "qm" in the command refers to the QEMU-based virtualization implemented in PVE. QEMU is an open-source emulator and virtualization tool that enables running multiple computer operating systems on a single machine.

The "delsnapshot" part of the command refers to the action of deleting a snapshot of a VM. A snapshot is a saved state of the VM at a point in time, and it allows for quickly reverting to that point in time when needed. It can be useful for backing up or testing changes to a VM, but can also consume significant disk space over time.

Therefore, the "qm delsnapshot" command is used to delete a snapshot of a VM in Proxmox VE. To run this command, you need to specify the VM ID and the snapshot name as arguments. For example, "qm delsnapshot 100 my_snapshot" would delete the "my_snapshot" named snapshot of the VM with ID 100.

Once executed, the command will remove the snapshot from the VM's disk image and free up space on the server. It's worth noting that deleting a snapshot is irreversible, and any changes made since the snapshot was taken will be lost. Therefore, it's important to carefully choose which snapshots to delete and when. 

## tldr 
 
> Delete virtual machine snapshots.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Delete a snapshot:

`qm delsnapshot {{vm_id}} {{snapshot_name}}`

- Delete a snapshot from a configuration file (even if removing the disk snapshot fails):

`qm delsnapshot {{vm_id}} {{snapshot_name}} --force 1`
