# virsh 
## chatgpt 
`virsh` is a command-line tool used for managing and manipulating virtual machines and their associated components. It is a part of the Libvirt toolkit and is used to interact with the hypervisor and the virtualization technology used by the host operating system.

When used with various subcommands, `virsh` can perform a wide range of virtual machine management operations. These operations include creating, deleting, starting, shutting down, pausing, resuming, and configuring virtual machines.

Some common `virsh` subcommands are:

1. `list` - lists all virtual machines

2. `start` - starts a virtual machine

3. `shutdown` - shuts down a virtual machine

4. `suspend` - suspends a virtual machine

5. `resume` - resumes a virtual machine

6. `destroy` - forcefully shuts down a virtual machine

7. `undefine` - deletes a virtual machine's definition

Overall, `virsh` is a powerful command-line tool that allows users to manage virtual machines efficiently with a wide range of advanced features and customization options. 

## tldr 
 
> Manage virsh guest domains. (NOTE: 'guest_id' can be the id, name or UUID of the guest).
> Some subcommands such as `virsh list` have their own usage documentation.
> More information: <https://libvirt.org/virshcmdref.html>.

- Connect to a hypervisor session:

`virsh connect {{qemu:///system}}`

- List all domains:

`virsh list --all`

- Dump guest configuration file:

`virsh dumpxml {{guest_id}} > {{path/to/guest.xml}}`

- Create a guest from a configuration file:

`virsh create {{path/to/config_file.xml}}`

- Edit a guest's configuration file (editor can be changed with $EDITOR):

`virsh edit {{guest_id}}`

- Start/reboot/shutdown/suspend/resume a guest:

`virsh {{command}} {{guest_id}}`

- Save the current state of a guest to a file:

`virsh save {{guest_id}} {{filename}}`

- Delete a running guest:

`virsh destroy {{guest_id}} && virsh undefine {{guest_id}}`
