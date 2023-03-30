# vmware-checkvm 
## chatgpt 
The command "vmware-checkvm" is a Linux command that allows users to check if they are running a virtual machine on a VMware hypervisor.

When executed, the command performs a series of checks to determine the current environment and whether it is compatible with VMware. Some of the checks that are performed by this command include:

- Checking if the user has the necessary permissions to access the hypervisor
- Identifying the type of hypervisor that is currently in use
- Verifying if the system has the necessary software or kernel module to run VMware

The output of the "vmware-checkvm" command contains information about the status of the VMware environment, including whether it is running in a virtual machine or a physical machine, the type of hypervisor in use, and the version of the VMware tools installed on the system.

Overall, this command is useful for diagnosing issues related to VMware and ensuring that the necessary software and modules are in place for the hypervisor to function properly. 

## tldr 
 
> Checks to see if the current host is a VMware VM or not.
> More information: <https://manned.org/vmware-checkvm>.

- Return the current VMware software version (exit status determines whether the system is a VM or not):

`vmware-checkvm`

- Return the VMware hardware version:

`vmware-checkvm -h`
