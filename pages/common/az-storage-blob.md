# az storage blob 
## chatgpt 
The `az storage blob` command is a sub-command under `az storage` command group in Azure CLI. It is used to interact with Azure Storage blobs, which are objects in Blob storage that hold data. 

Syntax:
```
az storage blob {copy} {delete} {download} {exists} {metadata} {show} {snapshot} {set-tier} {undelete} {upload} [OPTIONS]
```

Sub-commands:

- `copy`: Copies a blob to a destination blob within or across storage accounts.
- `delete`: Deletes a blob from the storage account.
- `download`: Downloads a blob to a file path on the local machine.
- `exists`: Checks whether a blob exists in the storage account.
- `metadata`: Manage blob metadata.
- `show`: Returns details about a blob in the storage account.
- `snapshot`: Manage blob snapshots.
- `set-tier`: Sets the tier for a blob.
- `undelete`: Restores a deleted blob.
- `upload`: Uploads a file or data to a blob in the storage account.

Options:
```
--account-name           # Name of the storage account.
--account-key            # Access key for the storage account.
--connection-string      # Connection string for the storage account.
--container-name         # Name of the container.
--dryrun                 # Shows the summary of the operation that would occur without actually performing it.
--lease-duration         # Specifies the duration of the lease in seconds.
--lease-break-period     # Specifies the time interval allowed for the lease to break.
--lease-id               # The lease ID of the blob.
--metadata               # Metadata in space-separated 'key=value' pairs. This overwrites any existing metadata.
--name                   # Name of the blob.
--pattern                # Pattern for the blob name. Can include '*' or '?' as wildcards.
--prefix                 # Prefix for the blob name.
--snapshot               # The blob snapshot for blob operations.
--source-blob            # The source blob URL used as source for the copy operation.
--source-container       # The container name used as source for the copy operation.
--source-uri             # The source blob URI used as source for the copy operation.
--start-time             # Specify the start time for conditional requests as milliseconds since the epoch.
--subscription           # Name or ID of the target subscription.
--timeout                # The timeout parameter is expressed in seconds.
--type                   # Indicator that the storage account creating the blob is a hierarchical namespace account.
--url                    # Fully-qualified URL of the blob.
--version-id             # The version ID of the blob.
```

Examples:

1. To upload a file to a blob in an Azure Storage account:
```
az storage blob upload --account-name mystorageaccount --account-key account_key --container-name mycontainer --name myblob --type block --source /path/to/file
```

2. To check if a blob exists in a container:
```
az storage blob exists --account-name mystorageaccount --account-key account_key --container-name mycontainer --name myblob
```

3. To copy a blob to a destination:
```
az storage blob copy start-batch --destination-container mydestinationcontainer --destination-blob mydestinationblob --source-container mysourcecontainer --source-blob mysourceblob --account-name mystorageaccount --account-key account_key
```

4. To delete a blob within a container:
```
az storage blob delete --account-name mystorageaccount --account-key account_key --container-name mycontainer --name myblob
```

5. To download a blob to a file path on the local machine:
```
az storage blob download --account-name mystorageaccount --account-key account_key --container-name mycontainer --name myblob --file /path/to/local/file
``` 

## tldr 
 
> Manage blob storage containers and objects in Azure.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/storage/blob>.

- Download a blob to a file path:

`az storage blob download --account-name {{storage_account_name}} --account-key {{storage_account_key}} -c {{container_name}} -n {{path/to/blob}} -f {{path/to/local_file}}`

- Download blobs from a blob container recursively:

`az storage blob download-batch --account-name {{storage_account_name}} --account-key {{storage_account_key}} -s {{container_name}} -d {{path/to/remote}} --pattern {{filename_regex}} --destination {{path/to/destination}}`

- Upload a local file to blob storage:

`az storage blob upload --account-name {{storage_account_name}} --account-key {{storage_account_key}} -c {{container_name}} -n {{path/to/blob}} -f {{path/to/local_file}}`

- Delete a blob object:

`az storage blob delete --account-name {{storage_account_name}} --account-key {{storage_account_key}} -c {{container_name}} -n {{path/to/blob}}`

- Generate a shared access signature for a blob:

`az storage blob generate-sas --account-name {{storage_account_name}} --account-key {{storage_account_key}} -c {{container_name}} -n {{path/to/blob}} --permissions {{permission_set}} --expiry {{Y-m-d'T'H:M'Z'}} --https-only`
