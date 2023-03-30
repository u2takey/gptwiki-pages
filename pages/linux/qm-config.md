# qm config 
## chatgpt 
The "qm config" command is a command that is used in the context of the QEMU virtual machine. QEMU is a free and open source emulator and virtualizer that can run different operating systems, including Linux, Windows, and macOS.

The "qm config" command allows you to view and modify the configuration of a QEMU virtual machine. When you run this command, you will be presented with a listing of the current configuration settings for your virtual machine.

The configuration settings that you can modify with the "qm config" command include the number of CPUs and the amount of RAM allocated to the virtual machine. You can also configure the virtual network interfaces and the storage options for the virtual machine.

Here is an example of how to use the "qm config" command:

qm config <vmid>

In this command, "vmid" is the virtual machine ID. You can find the ID of your virtual machine by running the "qm list" command.

When you run this command, you will be prompted to enter the password for your Proxmox VE host. Once you enter the correct password, you will be presented with a menu of options to view and modify the configuration settings for your virtual machine.

Overall, the "qm config" command is a useful tool for managing and configuring your QEMU virtual machines. 

## tldr 
 
> Display the virtual machine configuration with pending configuration changes applied.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Display the virtual machine configuration:

`qm config {{vm_id}}`

- Display the current configuration values instead of pending values for the virtual machine:

`qm config --current {{true}} {{vm_id}}`

- Fetch the configuration values from the given snapshot:

`qm config --snapshot {{snapshot_name}} {{vm_id}}`
