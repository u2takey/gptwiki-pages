# virsh pool-undefine 
## chatgpt 
The `virsh pool-undefine` command is used to undefine or delete a storage pool from the libvirt hypervisor. Here is a breakdown of each component of the command:

- `virsh`: This is the command-line tool used to interact with the libvirt hypervisor.
- `pool-undefine`: This is the subcommand used to delete a storage pool.

When you execute the `virsh pool-undefine` command, the hypervisor will search for the specified storage pool and attempt to delete it. If the operation is successful, the storage pool will be removed from the libvirt system and its resources will be freed up.

It is important to note that any data stored within the pool will also be lost, so you should be absolutely certain that you want to remove the pool before executing this command. Additionally, you should ensure that no guests are currently using the storage pool, as this could lead to data loss or corruption. 

## tldr 
 
> Delete the configuration file in `/etc/libvirt/storage` for a stopped virtual machine storage pool.
> See also: `virsh`, `virsh-pool-destroy`.
> More information: <https://manned.org/virsh>.

- Delete the configuration for the storage pool specified name or UUID (determine using `virsh pool-list`):

`virsh pool-undefine --pool {{name|uuid}}`
