# qm resume 
## chatgpt 
The command "qm resume" typically refers to the "resume" operation in the QEMU Manager (QM) software, which is a graphical user interface (GUI) for the QEMU emulator. This command is typically used to resume a suspended or paused virtual machine (VM) in QEMU.

When a VM is running in QEMU, it may be suspended or paused at any time, either manually by the user or automatically by the system. A suspended or paused VM is not running, but it is also not shut down completely. It is in a suspended state, waiting for the user to resume it.

To resume a suspended or paused VM in QEMU using the "qm resume" command, the user must first select the VM in the QEMU Manager interface, then click on the "resume" button or select the "resume" option from the menu. This will cause QEMU to start running the VM again from the point where it was suspended or paused, allowing the user to continue using the VM as normal.

Overall, the "qm resume" command is a simple and straightforward operation that allows users to easily resume a suspended or paused VM in QEMU using the QEMU Manager software. 

## tldr 
 
> Resume a virtual machine.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Resume a specific virtual machine:

`qm resume {{vm_id}}`

- Resume a specific virtual machine ignoring locks (requires root):

`sudo qm resume {{vm_id}} --skiplock true`
