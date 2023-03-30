# az storage container 
## chatgpt 
The 'az storage container' command is used to interact with Azure Storage containers, which are used to store and manage files and data in the cloud. The command includes several sub-commands that can be used to perform various actions:

- create: Creates a new container within a specified storage account.
- delete: Deletes a container.
- list: Lists all containers within a specified storage account.
- metadata: Allows for the addition, modification, or removal of metadata for a container.
- show: Shows the properties for a particular container.
- stats: Shows usage statistics for a container.
- legal-hold: Allows for the setting or clearing of legal hold on a container.
- immutability-policy: Allows for the creation, updating, or deletion of immutability policies for a container.

Each of these sub-commands requires different parameters to provide the necessary information to execute the desired action. For example, the 'create' sub-command requires a storage account name, a container name, and authentication credentials. The 'list' sub-command only requires the storage account name and authentication credentials.

Overall, the 'az storage container' command provides a simple and efficient way to manage Azure Storage containers via the command line interface. 

## tldr 
 
> Manage blob storage containers in Azure.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/storage/container>.

- Create a container in a storage account:

`az storage container create --account-name {{storage_account_name}} --name {{container_name}} --public-access {{access_level}} --fail-on-exist`

- Generate a shared access signature for the container:

`az storage container generate-sas --account-name {{storage_account_name}} --name {{container_name}} --permissions {{sas_permissions}} --expiry {{expiry_date}} --https-only`

- List containers in a storage account:

`az storage container list --account-name {{storage_account_name}} --prefix {{filter_prefix}}`

- Mark the specified container for deletion:

`az storage container delete --account-name {{storage_account_name}} --name {{container_name}} --fail-not-exist`
