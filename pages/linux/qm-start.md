# qm start 
## chatgpt 
The "qm start" command is a Proxmox Virtual Environment (PVE) command used to start a virtual machine (VM) that has been previously created and configured in the PVE. 

Here is a detailed explanation of the command:

- "qm" stands for "QEMU machine" and is the main command used to manage virtual machines in PVE.
- "start" is a sub-command that instructs PVE to start the VM with the specified ID.
- The ID can be a number or a name associated with the VM.
- When the "qm start" command is executed, PVE sends the start signal to QEMU, which in turn boots up the VM and starts the operating system.
- The VM must be in a stopped state (not running) in order for the "qm start" command to work.
- Depending on the VM's configuration, starting may take a few seconds up to a minute.
- The command can be run from the PVE web interface, the PVE command line interface (CLI), or remotely through SSH or other means.
- The "qm start" command can be combined with other options and parameters, such as "-daemonize" to start the VM in the background or "-boot" to specify which boot device to use.
- In summary, "qm start" is a simple yet powerful command that allows PVE administrators to start virtual machines on-demand, providing flexible and scalable computing resources on their Proxmox cluster. 

## tldr 
 
> Start a virtual machine on QEMU/KVM Virtual Machine Manager.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Start a specific virtual machine:

`qm start {{100}}`

- Specify the QEMU machine type (i.e. the CPU to emulate):

`qm start {{100}} --machine {{q35}}`

- Start a specific virtual machine with a timeout in 60 seconds:

`qm start {{100}} --timeout {{60}}`
