# VBoxManage 
## chatgpt 
VBoxManage is a command-line utility that is used to manage virtual machines in VirtualBox. It allows users to create, configure, and manage virtual machines, as well as their virtual hard disks, network interfaces, and other resources.

Syntax: VBoxManage [OPTIONS] COMMAND [ARGS]

The command consists of two parts:

1. OPTIONS: These are optional parameters that can be used to modify the behavior of the VBoxManage command. Examples of options include "--version" (displays the version number of VirtualBox), "--help" (displays the help message), and "--startvm" (starts a virtual machine).

2. COMMAND: This is the main action that you want to perform using VBoxManage. Examples of commands include "createvm" (creates a new virtual machine), "modifyvm" (modifies the configuration of an existing virtual machine), and "clonehd" (creates a copy of a virtual hard disk).

Some other important commands in VBoxManage are:

- startvm: Starts a virtual machine.
- controlvm: Controls a running virtual machine, such as pausing or resuming it.
- list: Lists the available virtual machines and their properties.
- snapshot: Allows users to take and manage snapshots of virtual machines.
- storageattach: Attaches a virtual storage device to a virtual machine.
- natnetwork: Configures a NAT network for the virtual machines to connect to the host and to each other.

VBoxManage is a powerful tool for managing virtual machines in VirtualBox, and it is essential for anyone who wants to customize and control their virtual machines from the command line. 

## tldr 
 
> Command-line interface to VirtualBox.
> Includes all the functionality of the GUI and more.
> More information: <https://www.virtualbox.org/manual/ch08.html#vboxmanage-intro>.

- List all VirtualBox virtual machines:

`VBoxManage list vms`

- Show information about a particular virtual machine:

`VBoxManage showvminfo {{name|uuid}}`

- Start a virtual machine:

`VBoxManage startvm {{name|uuid}}`

- Start a virtual machine in headless mode:

`VBoxManage startvm {{name|uuid}} --type headless`

- Shutdown the virtual machine and save its current state:

`VBoxManage controlvm {{name|uuid}} savestate`

- Shutdown down the virtual machine without saving its state:

`VBoxManage controlvm {{name|uuid}} poweroff`

- Update VBox extension packs:

`VBoxManage extpack install --replace {{VboxExtensionPackFileName}}`
