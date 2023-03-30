# virt-clone 
## chatgpt 
The virt-clone command is used in virtualization to create a clone or copy of an existing virtual machine (VM) in order to create a new VM with identical configurations as the original. When a VM is cloned, the clone inherits all the settings and properties of the original VM, thus allowing you to create multiple copies of an existing VM. Virt-clone can be used on a host machine running the KVM or QEMU hypervisor, and it works by copying the disk image of the original VM to create a new one. 

The basic syntax of the virt-clone command is as follows:
```
virt-clone --original <name> --name <new_name> [--auto-clone]
```
Where:
- `--original`: Specifies the name of the original virtual machine to be cloned.
- `--name`: Specifies the name of the new cloned virtual machine.
- `--auto-clone`: Specifies that the clone should be automatically configured and started after creation.

For example, if you want to clone a virtual machine named "vm1" and create a new VM called "vm2", you would use the following command:
```
virt-clone --original vm1 --name vm2
```

Other parameters can also be used with the virt-clone command to customize the clone process, such as specifying a new disk image location, changing the network settings or adding custom configurations. Overall, the virt-clone command is a handy tool for creating identical copies of existing virtual machines, which can be helpful especially in situations where you need several VMs with the same configurations for testing or development purposes. 

## tldr 
 
> Clone a libvirt virtual machine.
> More information: <https://manned.org/virt-clone>.

- Clone a virtual machine and automatically generate a new name, storage path, and MAC address:

`virt-clone --original {{vm_name}} --auto-clone`

- Clone a virtual machine and specify the new name, storage path, and MAC address:

`virt-clone --original {{vm_name}} --name {{new_vm_name}} --file {{path/to/new_storage}} --mac {{ff:ff:ff:ff:ff:ff|RANDOM}}`
