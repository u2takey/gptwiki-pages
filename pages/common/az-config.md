# az config 
## chatgpt 
The "az config" command is a command-line tool provided by the Azure CLI (Command-Line Interface) that is used to manage Azure CLI configuration settings. It helps you to set and manage various configurations such as default output format, default subscription, custom endpoint configurations etc. Here's a brief description of what this command does:

The "az config" command provides various sub-commands to manage configuration settings, such as:

1. "set" sub-command allows you to set a configuration value for a specific configuration parameter. For example, you can set the default output format to JSON or set a custom endpoint for Azure.

2. "get" sub-command allows you to retrieve the value of a specific configuration parameter. For example, you can get the current default subscription ID.

3. "list" sub-command allows you to list all the configuration parameters and their values.

4. "unset" sub-command allows you to remove a specific configuration value.

Overall, the "az config" command is used to manage global configuration settings for Azure CLI commands. It helps you to easily configure your CLI environment, and ensures that your Azure resources are accessed using the right credentials and settings. 

## tldr 
 
> Manage Azure CLI configuration.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/config>.

- Print all configurations:

`az config get`

- Print configurations for a specific section:

`az config get {{section_name}}`

- Set a configuration:

`az config set {{configuration_name}}={{value}}`

- Unset a configuration:

`az config unset {{configuration_name}}`
