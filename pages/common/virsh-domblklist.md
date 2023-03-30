# virsh-domblklist 
## chatgpt 
The `virsh-domblklist` command is used to list the block devices (such as hard disk, CD/DVD drive) attached to a particular virtual machine.

The command syntax is as follows:

`virsh domblklist <domain>`

where `<domain>` is the name or ID of the virtual machine for which you want to list the block devices.

The output of the command includes the source of the block device (such as a file or a physical device), the target name (such as hda or hdc), and the type of device (such as disk or cdrom).

The `virsh domblklist` command can be useful for troubleshooting and managing virtual machine storage. For example, you can use it to identify the source file of a virtual hard disk or to remove a CD/DVD image attached to a virtual machine. 

## tldr 
 
> List information about block devices associated with a virtual machine.
> See also: `virsh`.
> More information: <https://manned.org/virsh>.

- List the target name and source path of the block devices:

`virsh domblklist --domain {{vm_name}}`

- List the disk type and device value as well as the target name and source path:

`virsh domblklist --domain {{vm_name}} --details`
