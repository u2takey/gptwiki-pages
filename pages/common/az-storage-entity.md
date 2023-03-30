# az storage entity 
## chatgpt 
The `az storage entity` command is a sub-command of the Azure CLI (command-line interface) tool that is used to manage entities in Azure Storage service. Here's a brief explanation of this command:

1. The `az` command is used to interact with Azure resources through Azure CLI.

2. The `storage` command is used to interact with Azure Storage service, which includes multiple services like blobs, queues, tables, and files.

3. The `entity` command is used to interact with entities in Azure Storage tables.

Azure Storage tables are NoSQL data stores that can be used to store structured data. An entity is a single row in a table, which contains multiple properties (columns). Each entity has a unique partition key and row key that identify its location in the table.

The `az storage entity` command provides several sub-commands that allow users to perform different actions on entities in a table. For example, you can use the `create` sub-command to create a new entity, the `show` sub-command to retrieve an entity, the `list` sub-command to list all entities in a table, and the `delete` sub-command to delete an entity.

Overall, the `az storage entity` command is a useful tool for managing entities in Azure Storage tables through the Azure CLI. 

## tldr 
 
> Manage Azure Table storage entities.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/storage/entity>.

- Insert an entity into a table:

`az storage entity insert --entity {{space_separated_key_value_pairs}} --table-name {{table_name}} --account-name {{storage_account_name}} --account-key {{storage_account_key}}`

- Delete an existing entity from a table:

`az storage entity delete --partition-key {{partition_key}} --row-key {{row_key}} --table-name {{table_name}} --account-name {{storage_account_name}} --account-key {{storage_account_key}}`

- Update an existing entity by merging its properties:

`az storage entity merge --entity {{space_separated_key_value_pairs}} --table-name {{table_name}} --account-name {{storage_account_name}} --account-key {{storage_account_key}}`

- List entities which satisfy a query:

`az storage entity query --filter {{query_filter}} --table-name {{table_name}} --account-name {{storage_account_name}} --account-key {{storage_account_key}}`

- Get an entity from the specified table:

`az storage entity show --partition-key {{partition_key}} --row-key {{row_key}} --table-name {{table_name}} --account-name {{storage_account_name}} --account-key {{storage_account_key}}`
