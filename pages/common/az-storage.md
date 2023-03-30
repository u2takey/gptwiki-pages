# az storage 
## chatgpt 
The command "az storage" is a command-line interface (CLI) command for managing Azure Storage resources. Azure Storage is a cloud-based storage solution that provides various types of storage services, like Blob storage, Queue storage, Table storage, and File storage for storing and accessing large amounts of data in the cloud.

The "az storage" command enables the user to create, manage, and monitor Azure Storage resources using the Azure CLI. It provides a wide range of subcommands that enable the user to perform various storage-related tasks, such as creating and managing storage accounts, creating and managing containers, uploading and downloading files, managing permissions, and retrieving metrics and logs for storage resources.

Some of the commonly used subcommands for "az storage" are:

- "az storage account create": This command creates a new storage account in Azure.
- "az storage container create": This command creates a new container in a storage account.
- "az storage blob upload": This command uploads a file to a container in a storage account.
- "az storage blob download": This command downloads a file from a container in a storage account.
- "az storage account keys list": This command lists the access keys for a storage account.
- "az storage blob metadata show": This command shows the metadata for a blob in a container.

In summary, the "az storage" command is used to manage Azure Storage resources using Azure CLI, and provides various subcommands to perform storage-related operations efficiently. 

## tldr 
 
> Manage Azure Cloud Storage resources.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/storage>.

- Create a storage account:

`az storage account create -g {{group_name}} -n {{account_name}} -l {{location}} --sku {{account_sku}}`

- List all storage accounts in a resource group:

`az storage account list -g {{group_name}}`

- List the access keys for a storage account:

`az storage account keys list -g {{group_name}} -n {{account_name}}`

- Delete a storage account:

`az storage account delete -g {{group_name}} -n {{account_name}}`

- Update the minimum tls version setting for a storage account:

`az storage account update --min-tls-version TLS1_2 -g {{group_name}} -n {{account_name}}`
