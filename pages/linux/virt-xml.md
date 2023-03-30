# virt-xml 
## chatgpt 
virt-xml is a command-line tool that is used to manage and modify libvirt XML configuration files. Libvirt is an open-source API, daemon, and management tool for managing virtualization platforms such as KVM, QEMU, Xen, and LXC.

The virt-xml command can be used to create, read, update, and delete XML configuration files for virtual machines, network interfaces, storage volumes, and other virtual resources. Some of the common operations that can be performed using virt-xml include:

1. Creating a new XML configuration file for a virtual machine or a network interface.
2. Editing an existing XML configuration file to modify the virtual machine's hardware settings, such as CPU, RAM, disk space and network interface configuration.
3. Deleting an existing XML configuration file for a virtual machine, network interface or storage volume.
4. Querying the configuration details of a virtual machine or network interface.

The virt-xml command requires root privileges to run and can be installed on a Linux system that has Libvirt installed. Some of the commonly used options with the virt-xml command include:

- --connect: This option is used to specify the URI of the hypervisor connection. By default, it connects to the local hypervisor service.
- --edit: This option is used to edit the XML configuration file.
- --show: This option is used to display the XML configuration file in its current state.
- --name: This option is used to specify the name of the virtual machine or network interface. If not specified, it takes the first virtual machine or network interface in the XML file.
- --update: This option is used to update the XML configuration file with the new settings.

Overall, the virt-xml command is a powerful tool for managing and modifying Libvirt XML configuration files for virtual machines and other virtual resources. 

## tldr 
 
> Edit libvirt Domain XML files with explicit command line options.
> NOTE: 'domain' refers to the name, UUID or ID for the existing VMs (See: tldr virsh).
> More information: <https://github.com/virt-manager/virt-manager/blob/main/man/virt-xml.rst>.

- List all the suboptions for a specific option:

`virt-xml --{{option}}=?`

- List all the suboptions for disk, network, and boot:

`virt-xml --disk=? --network=? --boot=?`

- Edit a value for a specific domain:

`virt-xml {{domain}} --edit --{{option}} {{suboption}}={{new_value}}`

- Change the description for a specific domain:

`virt-xml {{domain}} --edit --metadata description="{{new_description}}"`

- Enable/Disable the boot device menu for a specific domain:

`virt-xml {{domain}} --edit --boot bootmenu={{on|off}}`

- Attach host USB hub to a running VM (See: tldr lsusb):

`virt-xml {{domain}} --update --add-device --hostdev {{bus}}.{{device}}`
