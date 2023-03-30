# qm wait 
## chatgpt 
The command "qm wait" is often used in the context of the Linux KVM (Kernel-based Virtual Machine) hypervisor, which is used to create and manage virtual machines on a Linux system. 

The "qm wait" command is used to pause a particular virtual machine, identified by its ID or name, until all of its associated processes have finished executing. This is especially useful when performing maintenance or updates on the host system, as it ensures that all processes within the virtual machine have finished before the virtual machine is shut down or restarted.

When the "qm wait" command is executed, the specified virtual machine will enter a pause state and remain in that state until all of its processes have completed. Once all processes have finished, the virtual machine will automatically resume running. During this time, the virtual machine will not consume any CPU or memory resources, but will remain in the memory of the host system.

Overall, the "qm wait" command is a useful tool for managing virtual machines on a Linux KVM hypervisor, helping to ensure smooth and efficient performance of virtual machines on the host system. 

## tldr 
 
> Wait until the virtual machine is stopped.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Wait until the virtual machine is stopped:

`qm wait {{vm_id}}`

- Wait until the virtual machine is stopped with a 10 second timeout:

`qm wait --timeout {{10}} {{vm_id}}`

- Send a shutdown request, then wait until the virtual machine is stopped with a 10 second timeout:

`qm shutdown {{vm_id}} && qm wait --timeout {{10}} {{vm_id}}`
