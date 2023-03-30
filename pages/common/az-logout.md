# az logout 
## chatgpt 
The command "az logout" is used to log out of the current Azure account that is being used via the Azure CLI (Command Line Interface). This command will remove the access token and refresh token from the system, which means the user will not be able to access any resources of Azure that requires authentication.

The command is run using the "az" command followed by "logout" keyword, as shown below:

az logout

The command does not have any additional parameters or arguments.

Note that after running this command, the user will be logged out of all subscriptions and tenants associated with the current Azure account. The user will need to log in again using the "az login" command to access the Azure resources. 

## tldr 
 
> Log out from an Azure subscription.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/reference-index#az_logout>.

- Log out from the active account:

`az logout`

- Log out a specific username:

`az logout --username {{alias@somedomain.com}}`
