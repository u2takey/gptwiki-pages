# virsh pool-autostart 
## chatgpt 
The `virsh pool-autostart` command is used to configure the automatic startup of a storage pool when the host machine boots up. 

The "virsh" part of the command refers to the Virtualization Shell, which is a command-line tool used to manage virtual machines and storage pools on a host.

The "pool-autostart" part of the command specifies the action being executed, which is configuring the automatic startup of a storage pool.

When you run the `virsh pool-autostart` command followed by the name of the storage pool you want to configure, the Virtualization Shell will modify the configuration file for that pool to set the "autostart" property to "yes". 

This means that when the host machine starts up, the storage pool will automatically be started, without any additional user input required.

Overall, the `virsh pool-autostart` command is a useful tool for managing the startup behavior of storage pools on a virtualization host. By automating the startup process, it can help streamline the management of virtual environments and improve efficiency. 

## tldr 
 
> Enable or disable autostart for a virtual machine storage pool.
> See also: `virsh`.
> More information: <https://manned.org/virsh>.

- Enable autostart for the storage pool specified by name or UUID (determine using `virsh pool-list`):

`virsh pool-autostart --pool {{name|uuid}}`

- Disable autostart for the storage pool specified by name or UUID:

`virsh pool-autostart --pool {{name|uuid}} --disable`
