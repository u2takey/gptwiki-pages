# qm rescan 
## chatgpt 
The "qm rescan" command is a command that is commonly used in virtualized environments. It is used to manually rescan the storage devices that are attached to the virtual machine host in order to detect any new storage devices that have been attached or to update any changes that have been made to the existing ones.

When you run the "qm rescan" command, it will instruct your virtual machine host to scan for any new or updated storage devices that are connected to the system. Once the scanning process is completed, the virtual machine host will be able to recognize any changes made to existing storage devices or will detect any new storage devices that have been connected to the system.

This is a useful command to run when you have made changes or additions to the storage devices that are attached to your virtual machine host, as it ensures that your virtual machines have the most recent information about the storage devices available to them. This can be particularly important when you are working with sensitive data or applications that require high levels of integrity and security. 

## tldr 
 
> Rescan all storages and update disk sizes and unused disk images of a virtual machine.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Rescan all storages and update disk sizes and unused disk images of a specific virtual machine:

`qm rescan {{vm_id}}`

- Perform a dry-run of rescan on a specific virtual machine and do not write any changes to configurations:

`qm rescan --dryrun {{true}} {{vm_id}}`
