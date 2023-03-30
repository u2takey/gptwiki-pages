# az account 
## chatgpt 
The `az account` command is used with the Azure Command-Line Interface (CLI) and is used to manage your Azure account. With this command, you can view the current subscription and tenant that you are working in, switch between subscriptions and tenants, and also list all subscriptions and tenants that you have access to.

Some of the commonly used arguments with the `az account` command are:

- `list`: This argument is used to list all the subscriptions that you have access to.

- `show`: This argument is used to display the details of the current subscription and tenant that you are working in.

- `set`: This argument is used to switch between subscriptions or tenants. You can specify the subscription or tenant ID to switch to.

- `create`: This argument is used to create a new Azure account.

- `delete`: This argument is used to delete an Azure account.

Overall, the `az account` command is a key command to manage your Azure account and is used in various scenarios. 

## tldr 
 
> Manage Azure subscription information.
> Part of `az`, the command-line client for Microsoft Azure.
> More information: <https://learn.microsoft.com/cli/azure/account>.

- Print a list of subscriptions for the logged in account:

`az account list`

- Set a `subscription` to be the currently active subscription:

`az account set --subscription {{subscription_id}}`

- List supported regions for the currently active subscription:

`az account list-locations`

- Print an access token to be used with `MS Graph API`:

`az account get-access-token --resource-type {{ms-graph}}`

- Print details of the currently active subscription in a specific format:

`az account show --output {{json|tsv|table|yaml}}`
