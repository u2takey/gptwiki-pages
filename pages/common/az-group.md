# az group 
## chatgpt 
The "az group" command is a part of the Azure CLI (Command-Line Interface), which is used for managing and deploying resources in Microsoft Azure. 

The "az group" command is used to create, retrieve, update, or delete resource groups in Azure. A resource group is a logical container used to organize and manage Azure resources, such as virtual machines, storage accounts, and networking resources.

The command can be used with a variety of sub-commands:

- "create": This sub-command is used to create a new resource group.
- "show": This sub-command is used to display the details of an existing resource group.
- "list": This sub-command is used to display a list of all the resource groups in the current subscription.
- "update": This sub-command is used to modify the properties of an existing resource group.
- "delete": This sub-command is used to delete an existing resource group.

In order to use the "az group" command, you must have the Azure CLI installed and logged into your Azure account. The syntax for using the command varies depending on the desired sub-command and any required parameters or arguments. 

Overall, the "az group" command is a useful tool for managing Azure resource groups and organizing resources for efficient management and deployment in the Azure cloud platform. 

## tldr 
 
> Manage resource groups and template deployments.
> Part of `azure-cli`.
> More information: <https://docs.microsoft.com/cli/azure/group>.

- Create a new resource group:

`az group create --name {{name}} --location {{location}}`

- Check if a resource group exists:

`az group exists --name {{name}}`

- Delete a resource group:

`az group delete --name {{name}}`

- Wait until a condition of the resource group is met:

`az group wait --name {{name}} --{{created|deleted|exists|updated}}`
