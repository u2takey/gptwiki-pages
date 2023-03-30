# qm unlock 
## chatgpt 
The "qm unlock" command is used in the Proxmox Virtual Environment (PVE) to unlock a virtual machine (VM) that has been locked due to an action being performed on it or due to an error occurring. When a VM is locked, it cannot be powered on, migrated, or deleted until it is unlocked.

Here is how the "qm unlock" command works:

1. Log in to the PVE host using SSH or on the console.
2. Determine the VM ID of the VM that is locked by running the command "qm list".
3. Run the "qm unlock <VMID>" command, replacing <VMID> with the ID of the locked VM.
4. The command will remove any locks on the VM and allow you to power on, migrate, or delete it again.

It is important to note that using the "qm unlock" command can potentially cause data loss or corruption, especially if the VM was locked due to an error. Therefore, it is recommended to investigate the cause of the lock before unlocking the VM to prevent any data loss. 

## tldr 
 
> Unlock a virtual machine in QEMU/KVM Virtual Machine Manager.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Unlock a specific virtual machine:

`qm unlock {{vm_id}}`
