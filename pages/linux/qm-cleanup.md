# qm cleanup 
## chatgpt 
As an AI language model, I am not sure about the context and specific system where this command is being used. However, I can provide a general explanation of the possible meaning and purpose of the command "qm cleanup".

"qm cleanup" is likely a command that is related to cleaning up and optimizing the system's resources by removing unwanted or unnecessary files, folders, and processes. This command might be a script or a tool that performs a series of cleanup tasks, such as removing temporary files, uninstalling unused applications, deleting log files, clearing cache memory, and optimizing the system's performance.

In some cases, "qm cleanup" might be a command used in a specific application or program, where it performs cleanup tasks associated with that application. For instance, it can be used for cleaning up the virtual machines of a QEMU-KVM hypervisor.

Overall, the exact function and operation of the "qm cleanup" command can vary depending on its context and the system or application where it is being used. It is important to be cautious while using any cleanup command, as it can potentially delete important files and cause system instability. Hence it's recommended to take a backup before executing this command. 

## tldr 
 
> Clean up resources on QEMU/KVM Virtual Machine Manager like tap devices, VGPUs, etc.
> Called after a VM shuts down, crashes, etc.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Clean up resources:

`qm cleanup {{vm_id}} {{clean-shutdown}} {{guest-requested}}`
