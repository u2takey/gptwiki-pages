# qm clone 
## chatgpt 
The "qm clone" command is used in Proxmox Virtual Environment (PVE) to create a copy of a virtual machine (VM) for backup or migration purposes. The command takes the following syntax:

qm clone <vmid> <target_vm_name>

Where:

- "vmid" is the ID number of the VM to be cloned.
- "target_vm_name" is the desired name for the new cloned VM.

When executed, the "qm clone" command creates a fully functional copy of the selected VM, including its configuration settings, virtual disks, network settings, and attached devices. The cloned VM is created as a new independent entity in PVE, with a unique ID number and name of its own.

Some notable features of the "qm clone" command include:

- Cloning a VM is a quick and simple way to create a backup or replica of an existing VM. The cloned VM can be used for testing, development, or as a standby in case the original VM fails or becomes unavailable.
- The command can be executed either through the PVE web interface or via the command line interface (CLI). In the CLI, the command requires root access and must be run on the PVE host where the VM is located.
- The cloned VM inherits the hardware resources and system settings of the original VM, but it can be modified and customized independently.
- By default, the virtual disks of the cloned VM are stored in the same storage pool as the original VM. However, users can specify a different storage pool or increase/decrease the size of the virtual disks during the cloning process.
- Cloning a VM does not affect the original VM or its ongoing operations. However, to avoid conflicts, it is recommended to avoid running both the original and cloned VMs simultaneously on the same PVE host.
- The "qm clone" command is just one of several options for replicating VMs in PVE. Other options include backup/restore, live migration, and snapshotting. The choice of replication method depends on the specific requirements and constraints of the PVE environment. 

## tldr 
 
> Create a copy of virtual machine on QEMU/KVM Virtual Machine Manager.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Copy a virtual machine:

`qm copy {{vm_id}} {{new_vm_id}}`

- Copy a virtual machine using a specific name:

`qm copy {{vm_id}} {{new_vm_id}} --name {{name}}`

- Copy a virtual machine using a specific descriptionn:

`qm copy {{vm_id}} {{new_vm_id}} --description {{description}}`

- Copy a virtual machine creating a full copy of all disks:

`qm copy {{vm_id}} {{new_vm_id}} --full`

- Copy a virtual machine using a specific format for file storage (requires `--full`):

`qm copy {{vm_id}} {{new_vm_id}} --full --format {{qcow2|raw|vmdk}}`

- Copy a virtual machine then add it to a specific pool:

`qm copy {{vm_id}} {{new_vm_id}} --pool {{pool_name}}`
