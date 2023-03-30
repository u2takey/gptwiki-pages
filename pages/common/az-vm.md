# az vm 
## chatgpt 
The "az vm" command is part of the Azure CLI (Command-Line Interface) tool and is used to manage virtual machines (VMs) in Microsoft Azure. 

The command allows you to perform various operations on VMs such as creating, starting, stopping, deleting, resizing, and so on. 

Some common sub-commands that can be used with "az vm" include:

- create: This sub-command is used to create a new VM. It requires parameters such as a name, image, region, username, password, and size of the VM.
- start: This sub-command is used to start a stopped VM.
- stop: This sub-command is used to stop a running VM.
- delete: This sub-command is used to delete a VM.
- list: This sub-command is used to list all VMs in a resource group or subscription.

Overall, the "az vm" command is a powerful tool for managing virtual machines in Azure via the command line. 

## tldr 
 
> Manage virtual machines in Azure.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/vm>.

- List details of available Virtual Machines:

`az vm list`

- Create a virtual machine using the default Ubuntu image and generate ssh keys:

`az vm create --resource-group {{rg}} --name {{vm_name}} --image {{UbuntuLTS}} --admin-user {{azureuser}} --generate-ssh-keys`

- Stop a Virtual Machine:

`az vm stop --resource-group {{rg}} --name {{vm_name}}`

- Deallocate a Virtual Machine:

`az vm deallocate --resource-group {{rg}} --name {{vm_name}}`

- Start a Virtual Machine:

`az vm start --resource-group {{rg}} --name {{vm_name}}`

- Restart a Virtual Machine:

`az vm restart --resource-group {{rg}} --name {{vm_name}}`

- List VM images available in the Azure Marketplace:

`az vm image list`
