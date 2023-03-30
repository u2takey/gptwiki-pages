# az storage account 
## chatgpt 
az storage account is a command used in the Azure command-line interface (CLI) to manage and interact with Azure Storage accounts. This command can be used to create new storage accounts, update existing ones, view account details, and perform various administrative tasks related to storage.

The syntax for the command is as follows:

az storage account {create | delete | list | show | update} [options]

Each sub-command within the az storage account command has its own set of options and parameters. For example:
- az storage account create is used to create a new storage account. This command requires parameters such as the account name, resource group, and location of the account.
- az storage account delete is used to delete an existing storage account. This command requires the account name and resource group.
- az storage account list is used to view a list of all storage accounts in a given subscription or resource group.
- az storage account show is used to display the details of a specific storage account. This command requires the account name and resource group.
- az storage account update is used to update the properties of an existing storage account. This command requires parameters such as the account name and resource group, as well as the specific property to update.

Overall, the az storage account command provides administrators with a powerful set of tools for managing and manipulating Azure Storage accounts from the command line. 

## tldr 
 
> Manage storage accounts in Azure.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/storage/account>.

- Create an storage account:

`az storage account create --name {{storage_account_name}} --resource-group {{azure_resource_group}} --location {{azure_location}} --sku {{storage_account_sku}}`

- Generate a shared access signature for a specific storage account:

`az storage account generate-sas --account-name {{storage_account_name}} --name {{account_name}} --permissions {{sas_permissions}} --expiry {{expiry_date}} --services {{storage_services}} --resource-types {{resource_types}}`

- List storage accounts:

`az storage account list --resource-group {{azure_resource_group}}`

- Delete a specific storage account:

`az storage account delete --name {{storage_account_name}} --resource-group {{azure_resource_group}}`
