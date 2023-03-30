# virsh pool-list 
## chatgpt 
The command "virsh pool-list" is used in the context of KVM (Kernel-based Virtual Machine) hypervisor to list the available storage pools. 

Here is a detailed explanation of its components:

- "virsh" is the command-line tool used to manage and operate virtual machines on KVM hypervisor.
- "pool-list" is the specific command that is being used here to get the list of available storage pools.

This command will display a table of all the configured storage pools on the system, including their names, states, and paths. The output can be useful to check the status of the storage pools, to configure access privileges, or to troubleshoot potential issues. Alternately, you can use "virsh pool-info <poolname>" command to get more details about a specific storage pool. 

## tldr 
 
> List information about virtual machine storage pools.
> See also: `virsh`, `virsh-pool-autostart`, `virsh-pool-define-as`.
> More information: <https://manned.org/virsh>.

- List the name, state, and whether autostart is enabled or disabled for active storage pools:

`virsh pool-list`

- List information for active and inactive or just inactive storage pools:

`virsh pool-list --{{all|inactive}}`

- List extended information about persistence, capacity, allocation, and available space for active storage pools:

`virsh pool-list --details`

- List information for active storage pools with either autostart enabled or disabled:

`virsh pool-list --{{autostart|no-autostart}}`

- List information for active storage pools that are either persistent or transient:

`virsh pool-list --{{persistent|transient}}`

- List the name and UUID of active storage pools:

`virsh pool-list --name --uuid`
