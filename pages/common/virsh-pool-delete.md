# virsh pool-delete 
## chatgpt 
"virsh pool-delete" is a command used to delete a storage pool in the Virtualization environment managed by KVM (Kernel-based Virtual Machine) hypervisor. Storage pools are used to store virtual machine images, ISO files, and other storage objects in KVM.

To use "virsh pool-delete" command, you need to have administrative privileges on the KVM host system. Here are the steps to use this command:

1. Open the terminal window on the KVM host system.
2. Type "virsh pool-list" command to see the list of available storage pools.
3. Identify the name of the storage pool you want to delete. Note that you cannot delete an active pool. So, make sure the pool is inactive.
4. Type "virsh pool-delete [pool-name]" command to delete the specified storage pool. Replace [pool-name] with the actual name of the pool you want to delete.
5. Press Enter to execute the command.
6. If successful, you will see a message confirming the deletion of the storage pool.

Note that deleting a storage pool will also delete all the objects (virtual machine images, ISO files, etc.) stored in it. So, make sure you have backed up any important data before deleting a storage pool. 

## tldr 
 
> Delete the underlying storage system of an inactive virtual machine storage pool.
> See also: `virsh`, `virsh-pool-destroy`, `virsh-pool-undefine`.
> More information: <https://manned.org/virsh>.

- Delete the underlying storage system for the storage pool specified by name or UUID (determine using `virsh pool-list`):

`virsh pool-delete --pool {{name|uuid}}`
