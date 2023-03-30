# azcopy 
## chatgpt 
Azcopy is a command-line tool developed by Microsoft that allows users to easily transfer data to and from Azure storage services. The command "azcopy" is used to invoke the tool and access its various functions.

The basic syntax of the command is as follows:

```
azcopy [command] [options]
```

The "command" parameter specifies the action to be performed, such as copying, downloading, or syncing data. The available commands include:

- copy: Copies data from a source to a destination.
- sync: Syncs the contents of a source with a destination.
- list: Lists the contents of a container or blob.
- remove: Deletes a container or blob.

The "options" parameter specifies additional settings for the command. These can include:

- Source and Destination URLs: The location of the data to be transferred and the location where it should be stored.
- Credentials: The username and password or SAS token required to access the source and destination.
- Transfer settings: Specifies the concurrency, chunk size, and other performance-related options.

Overall, the Azcopy command is a powerful and flexible tool for managing data in Azure storage services. It can be used to migrate data, backup data, and synchronize data between on-premises and cloud storage locations. 

## tldr 
 
> A file transfer tool for uploading to Azure Cloud Storage Accounts.
> More information: <https://learn.microsoft.com/azure/storage/common/storage-use-azcopy-v10>.

- Log in to an Azure Tenant:

`azopy login`

- Upload a local file:

`azcopy copy '{{path\to\source_file}}' 'https://{{storage_account_name}}.blob.core.windows.net/{{container_name}}/{{blob_name}}'`

- Upload files with `.txt` and `.jpg` extensions:

`azcopy copy '{{path\to\source_directory}}' 'https://{{storage_account_name}}.blob.core.windows.net/{{container_name}}' --include-pattern '{{*.txt;*.jpg}}'`

- Copy a container directly between two Azure storage accounts:

`azcopy copy 'https://{{source_storage_account_name}}.blob.core.windows.net/{{container_name}}' 'https://{{destination_storage_account_name}}.blob.core.windows.net/{{container_name}}'`

- Synchronize a local directory and delete files in the destination if they no longer exist in the source:

`azcopy sync '{{path\to\source_directory}}' 'https://{{storage_account_name}}.blob.core.windows.net/{{container_name}}' --recursive --delete-destination=true`

- Display detailed usage information:

`azcopy --help`
