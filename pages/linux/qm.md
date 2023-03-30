# qm 
## chatgpt 
The "qm" command is used in the Proxmox Virtual Environment (PVE) to manage and control virtual machines (VMs) that are hosted on the server. It stands for "QEMU Manager" and provides a way to perform various tasks related to the management of VMs.

The "qm" command can be used to perform a variety of tasks including creating and deleting VMs, starting and stopping VMs, and modifying VM configurations. Some common tasks that can be performed using the "qm" command include:

- Creating a new VM: The "qm create" command is used to create a new VM on the PVE server. This command requires specifying the VM ID, name, and type. For example, "qm create 100 --name my_vm --memory 1024 --net0 virtio,bridge=vmbr0" would create a new VM with an ID of 100, a name of "my_vm", 1GB of memory, and a network interface connected to the "vmbr0" bridge.

- Starting a VM: The "qm start" command is used to start a VM that is currently stopped. This command requires specifying the VM ID. For example, "qm start 100" would start the VM with an ID of 100.

- Stopping a VM: The "qm stop" command is used to stop a VM that is currently running. This command requires specifying the VM ID. For example, "qm stop 100" would stop the VM with an ID of 100.

- Modifying VM settings: The "qm set" command is used to modify the settings of an existing VM. This command requires specifying the VM ID and the settings to be modified. For example, "qm set 100 --memory 2048" would set the memory of the VM with an ID of 100 to 2GB.

Overall, the "qm" command provides a powerful way to manage VMs on a PVE server from the command line, allowing users to automate tasks and perform management tasks quickly and easily. 

## tldr 
 
> QEMU/KVM Virtual Machine Manager.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- List all virtual machines:

`qm list`

- Using an ISO file uploaded on the local storage, create a virtual machine with a 4 GB IDE disk on the `local-lvm` storage and an ID of 100:

`qm create {{100}} -ide0 {{local-lvm:4}} -net0 {{e1000}} -cdrom {{local:iso/proxmox-mailgateway_2.1.iso}}`

- Show the configuration of a virtual machine, specifying its ID:

`qm config {{100}}`

- Start a specific virtual machine:

`qm start {{100}}`

- Send a shutdown request, then wait until the virtual machine is stopped:

`qm shutdown {{100}} && qm wait {{100}}`

- Destroy a virtual machine and remove all related resources:

`qm destroy {{100}} --purge`
