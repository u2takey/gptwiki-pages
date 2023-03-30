# qm create 
## chatgpt 
The command "qm create" is used in the Proxmox VE virtualization environment to create a new virtual machine (VM). 

Here is a breakdown of the command:

- "qm" is the Proxmox command that manages virtual machines and containers.
- "create" is an argument that tells the "qm" command to create a new VM.

When you run "qm create", you will need to provide additional parameters to specify the details of the new virtual machine. These parameters include:

- A unique ID for the new virtual machine.
- The type of operating system and version to install.
- The amount of RAM and CPU resources to allocate to the virtual machine.
- The amount of virtual storage to allocate to the virtual machine.
- The network configuration for the virtual machine (such as the MAC address and IP address).

Once you have provided these parameters, the "qm create" command will create a new virtual machine based on your specifications. 

## tldr 
 
> Create or restore a virtual machine on QEMU/KVM Virtual Machine Manager.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Create a virtual machine:

`qm create {{100}}`

- Automatically start the machine after creation:

`qm create {{100}} --start 1`

- Specify the type of operating system on the machine:

`qm create {{100}} --ostype {{win10}}`

- Replace an existing machine (requires archiving it):

`qm create {{100}} --archive {{path/to/backup_file.tar}} --force 1`

- Specify a script that is executed automatically depending on the state of the virtual machine:

`qm create {{100}} --hookscript {{path/to/script.pl}}`
