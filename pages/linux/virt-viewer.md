# virt-viewer 
## chatgpt 
The "virt-viewer" command is used to launch the Virtual Machine Manager (VMM) graphical console, which allows the user to interact with a virtual machine running on a Linux host. This command is typically used by system administrators to manage virtual machines on their network.

When executed, the virt-viewer command opens a graphical window that displays the console of the selected virtual machine. From this console, the user can perform various actions such as starting and stopping the virtual machine, attaching and detaching virtual devices, viewing and modifying virtual machine settings, and monitoring system performance.

In order to use the virt-viewer command, the user must have permission to access the Virtual Machine Manager and the virtual machines it manages. Additionally, the command may require additional software packages to be installed on the system, such as the SPICE protocol driver or the VNC server.

Overall, the virt-viewer command provides a convenient and easy-to-use interface for managing virtual machines on a Linux network. 

## tldr 
 
> Minimal graphical interface for a virtual machine (VM).
> NOTE: 'domain' refers to the name, UUID or ID for the existing VMs (See: tldr virsh).
> More information: <https://manned.org/virt-viewer>.

- Launch `virt-viewer` with a prompt to select running virtual machines:

`virt-viewer`

- Launch `virt-viewer` for a specific virtual machine by ID, UUID or name:

`virt-viewer "{{domain}}"`

- Wait for a virtual machine to start and automatically reconnect if it shutdown and restarts:

`virt-viewer --reconnect --wait "{{domain}}"`

- Connect to a specific remote virtual machine over TLS:

`virt-viewer --connect "xen//{{url}}" "{{domain}}"`

- Connect to a specific remote virtual machine over SSH:

`virt-viewer --connect "qemu+ssh//{{username}}@{{url}}/system" "{{domain}}"`
