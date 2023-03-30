# qm guest exec-status 
## chatgpt 
The command "qm guest exec-status" is a Proxmox Virtual Environment (PVE) command that is used to show the status of a process or command that is currently running inside a guest operating system (VM) that is managed by the PVE. This command can be executed from the PVE host shell or from within a guest operating system.

Here is the breakdown of the command:

- "qm" stands for "Qemu Manager" which is a key component of the PVE virtualization platform. This command is used to manage Qemu-based virtual machines.
- "guest" refers to the guest operating system running inside a virtual machine managed by PVE.
- "exec-status" is a sub-command that displays the status of the command or process running inside the guest VM.

The "qm guest exec-status" command provides information about the status of the command or process running inside the virtual machine. This includes the name, process ID (PID), CPU usage, memory usage, and current status of the process. The command is useful for monitoring the performance of virtual machines and identifying any issues that may arise.

Overall, the "qm guest exec-status" command is a powerful tool for PVE administrators and users to manage virtual machines and troubleshoot issues. 

## tldr 
 
> Print the status of the given pid started by the guest-agent on QEMU/KVM Virtual Machine Manager.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Print the status of a specific PID:

`qm guest exec-status {{vm_id}} {{pid}}`
