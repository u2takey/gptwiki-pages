# az storage table 
## chatgpt 
The "az storage table" command is used to perform operations on tables in an Azure Storage account. This command is a part of the Azure CLI (Command-Line Interface) tool, which is used to manage Azure resources from a command-line interface.

The following are some of the common subcommands used with the "az storage table" command:

1. create: This subcommand is used to create a new table in an Azure Storage account. To create a table, you need to specify the name of the table, along with the account name and account key.

2. delete: This subcommand is used to delete a table from an Azure Storage account. To delete a table, you need to specify the name of the table, along with the account name and account key.

3. list: This subcommand is used to list all the tables in an Azure Storage account. To list tables, you need to specify the account name and account key.

4. show: This subcommand is used to show the details of a specific table in an Azure Storage account. To show the details of a table, you need to specify the name of the table, along with the account name and account key.

5. insert: This subcommand is used to insert a new entity (row) in a table. To insert an entity, you need to specify the partition key, row key, and the properties of the entity.

6. query: This subcommand is used to query the entities in a table. To query entities, you need to specify the partition key, row key, and the query conditions.

Overall, the "az storage table" command is a powerful tool that enables users to create, manage, and query tables in an Azure Storage account from the command-line interface. 

## tldr 
 
> Manage NoSQL key-value storage in Azure.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/storage/table>.

- Create a new table in the storage account:

`az storage table create --account-name {{storage_account_name}} --name {{table_name}} --fail-on-exist`

- Generate a shared access signature for the table:

`az storage table generate-sas --account-name {{storage_account_name}} --name {{table_name}} --permissions {{sas_permissions}} --expiry {{expiry_date}} --https-only`

- List tables in a storage account:

`az storage table list --account-name {{storage_account_name}}`

- Delete the specified table and any data it contains:

`az storage table delete --account-name {{storage_account_name}} --name {{table_name}} --fail-not-exist`
