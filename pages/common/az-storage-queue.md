# az storage queue 
## chatgpt 
The "az storage queue" command is used to manage Azure Storage Queues. It allows users to create, update, delete, list, and show properties of queues in their Azure Storage account. Here's a breakdown of some of the key parameters and options of the command:

- "az storage queue create": This sub-command creates a new queue in the specified storage account. Users can specify the name of the queue and any metadata to be associated with it. They can also set the queue's properties, such as the message time-to-live and the visibility timeout.
- "az storage queue update": This sub-command updates the properties of an existing queue in the specified storage account. Users can change the queue's metadata and properties, as well as its access policy.
- "az storage queue delete": This sub-command deletes a queue from the specified storage account. Users must provide the name of the queue to be deleted.
- "az storage queue list": This sub-command lists all the queues in the specified storage account. Users can specify parameters such as max results and continuation token to control the output.
- "az storage queue show": This sub-command shows the properties of a specified queue in the specified storage account. Users must provide the name of the queue to be shown.

Overall, the "az storage queue" command is a powerful tool for managing Azure Storage Queues, providing various options for creating, updating, deleting, and listing queues. 

## tldr 
 
> Manage storage queues in Azure.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/storage/queue>.

- Create a queue:

`az storage queue create --account-name {{storage_account_name}} --name {{queue_name}} --metadata {{queue_metadata}}`

- Generate a shared access signature for the queue:

`az storage queue generate-sas --account-name {{storage_account_name}} --name {{queue_name}} --permissions {{queue_permissions}} --expiry {{expiry_date}} --https-only`

- List queues in a storage account:

`az storage queue list --prefix {{filter_prefix}} --account-name {{storage_account_name}}`

- Delete the specified queue and any messages it contains:

`az storage queue delete --account-name {{storage_account_name}} --name {{queue_name}} --fail-not-exist`
