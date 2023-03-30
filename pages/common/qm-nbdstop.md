# qm nbdstop 
## chatgpt 
The command "qm nbdstop" is used to stop the Network Block Device (NBD) server for a virtual machine in the Proxmox Virtual Environment (PVE). 

Here is a brief explanation of the terms used in the command:

- qm: This stands for "Qemu Manager" and is a tool provided by PVE to manage virtual machines.
- nbdstop: This is the sub-command used with qm to stop the NBD server.

The NBD server is used to export virtual machine disks over the network, allowing remote clients to access these disks as if they were locally attached. By running this command, you can stop any NBD server associated with a particular virtual machine, freeing up network resources and preventing any unauthorized access to the machine's disks. 

To use the command, simply run "qm nbdstop" followed by the ID number of the virtual machine you wish to stop the NBD server for. For example, if the ID of your virtual machine is 100, you would enter "qm nbdstop 100". When you run this command, Proxmox will stop the NBD server associated with the virtual machine immediately. 

## tldr 
 
> Stop embedded nbd server.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Stop embedded nbd server:

`qm nbdstop {{VM_ID}}`
