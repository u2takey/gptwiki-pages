# virsh pool-info 
## chatgpt 
The "virsh pool-info" command is a command-line tool that is used to display the details of a storage pool created in a virtual environment using the libvirt API. The command provides information about the configuration and status of the storage pool.

The syntax of the command is as follows:

virsh pool-info [pool-name]

Here, the [pool-name] is the name of the storage pool that you want to display the information for. If you omit the pool name, the command will display the information for the default storage pool.

When you run the command, it will display the following information about the specified storage pool:

1. Name: The storage pool name.

2. UUID: The unique identifier used to identify the storage pool.

3. State: The current state of the storage pool, which can be "running", "paused", "shutdown", "creating", or "deleting".

4. Autostart: Indicates if the storage pool is set to automatically start at boot.

5. Persistent: Indicates if the storage pool configuration is saved between host reboots.

6. Capacity: The total capacity of the storage pool in bytes.

7. Allocation: The amount of storage currently used by the pool in bytes.

8. Available: The amount of free storage available in the pool in bytes.

In summary, the "virsh pool-info" command is a useful tool for obtaining information about a virtual storage pool in a libvirt virtualization environment. It helps administrators to monitor and manage storage resources efficiently. 

## tldr 
 
> List information about a virtual machine storage pool.
> See also: `virsh`.
> More information: <https://manned.org/virsh>.

- List the name, UUID, state, persistence type, autostart status, capacity, space allocated, and space available for the storage pool specified by name or UUID (determine using `virsh pool-list`):

`virsh pool-info --pool {{name|uuid}}`
