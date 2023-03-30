# qm migrate 
## chatgpt 
The "qm migrate" command is used in Proxmox Virtual Environment (PVE) to migrate a virtual machine (VM) from one PVE node to another. 

QM stands for "QEMU," which is the hypervisor used by PVE to create and manage virtual machines. 

The "migrate" command is used specifically for migration purposes. This command allows you to migrate a VM from one PVE host to another, without having to shut down the VM. 

To use the "qm migrate" command, you need to specify the following:

- The VM ID - This is the ID number of the VM you want to migrate.
- The target node - This is the IP address or hostname of the PVE node where you want to migrate the VM.

You can also provide some additional options, including:

- The migration type - There are three options for the migration type: live, safe, and offline. Live migration allows you to migrate a VM without shutting it down, while safe migration stops the VM briefly during migration to ensure data integrity. Offline migration shuts down the VM during migration.
- The storage type - You can choose which type of storage to use for migration: local, shared, or any.

After executing the "qm migrate" command, the VM will be moved from the source PVE node to the target PVE node. The VM's configuration, disk images, and memory state will be transferred over the network to the target node. Once the migration is complete, you can start the VM on the target node and it should resume running as if nothing happened. 

## tldr 
 
> Migrate a virtual machine.
> Used to create a new migration task.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Migrate a specific virtual machine:

`qm migrate {{vm_id}} {{target}}`

- Override the current I/O bandwidth limit with 10 KiB/s:

`qm migrate {{vm_id}} {{target}} --bwlimit 10`

- Allow migration of virtual machines using local devices (root only):

`qm migrate {{vm_id}} {{target}} --force true`

- Use online/live migration if a virtual machine is running:

`qm migrate {{vm_id}} {{target}} --online true`

- Enable live storage migration for local disks:

`qm migrate {{vm_id}} {{target}} --with-local-disks true`
