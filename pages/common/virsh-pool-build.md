# virsh pool-build 
## chatgpt 
The `virsh pool-build` is a command used to build a storage pool in the virtualization environment using the Virtualization shell tool called `virsh`. A storage pool is a logical container that holds and manages a group of storage volumes or files. The storage pool is created according to the specified properties of the pool, such as the name of the pool, the type of storage, the path of storage, etc. 

The `virsh pool-build` command takes one argument, which is the name of the pool that you want to create. For example, if you want to create a storage pool named "mypool", you will enter the following command:

`virsh pool-build mypool`

Once you run the command, Virsh will create the necessary files and directories to set up the new storage pool. The command will return an output message indicating that the storage pool has been successfully created, and you can then add storage volumes or files to the new pool as needed.

The `virsh pool-build` command can also take additional parameters to configure the storage pool, such as specifying the type of storage, the path to store the data, the access mode, and other options. The available options are dependent on the type of storage pool you are creating. You can use the `virsh help pool-build` command to get more information about using the `virsh pool-build` command or refer to the virsh documentation for more detailed instructions. 

## tldr 
 
> Build the underlying storage system for a virtual machine storage pool as defined in it's configuration file in `/etc/libvirt/storage`.
> See also: `virsh`, `virsh-pool-define-as`, `virsh-pool-start`.
> More information: <https://manned.org/virsh>.

- Build the storage pool specified by name or UUID (determine using `virsh pool-list`):

`virsh pool-build --pool {{name|uuid}}`
