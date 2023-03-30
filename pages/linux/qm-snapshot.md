# qm snapshot 
## chatgpt 
The "qm snapshot" command is used in the Proxmox Virtual Environment (PVE) to take a snapshot of a virtual machine (VM). A snapshot is essentially a copy of the VM's state at a particular point in time, including its disk and memory contents.

When executed, the "qm snapshot" command creates a new snapshot of the specified VM. It takes a "live" snapshot, which means that the VM does not need to be stopped or paused before the snapshot is taken. The command also allows several options to be specified, such as the snapshot name, description, and whether to include memory contents in the snapshot.

Snapshots are useful for several reasons. For example, they can be used to create a backup or point-in-time image of a VM that can be restored later if needed. They can also be used to test new configurations or to roll back changes made to a VM that have caused problems.

It is important to note that snapshots consume additional disk space, so it is recommended to delete them once they are no longer needed. They also have some performance overhead, so it is generally not recommended to keep a large number of snapshots for an extended period of time. 

## tldr 
 
> Create virtual machine snapshots.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Create a snapshot of a specific virtual machine:

`qm snapshot {{vm_id}} {{snapshot_name}}`

- Create a snapshot with a specific description:

`qm snapshot {{vm_id}} {{snapshot_name}} --description {{description}}`

- Create a snapshot including the vmstate:

`qm snapshot {{vm_id}} {{snapshot_name}} --description {{description}} --vmstate 1`
