# az term 
## chatgpt 
Sorry, as an AI language model, I don't have access to the system for executing commands, but I can explain what the "az term" command is used for in the Azure CLI tool.

The "az term" command in Azure CLI is used to manage Azure Resource Manager template specs. It allows creating, updating, viewing, importing, exporting and deleting term metadata, which defines how parameters of a template spec can be assigned values. The term is a JSON document that defines the structure of the parameter values, their types, descriptions, labels, and default values.

Here are some examples of using "az term" command:

- To create a new term metadata from a JSON file:
  az term create --name "myTerm" --term-file path/to/myTerm.json

- To update an existing term metadata:
  az term update --name "myTerm" --set "metadata.label='New Label'"

- To list all terms in the current subscription:
  az term list

- To export a term metadata to a JSON file:
  az term export --name "myTerm" --output file.json

- To delete a term metadata:
  az term delete --name "myTerm"

This command is useful when managing infrastructure as code in Azure, enabling efficient and consistent deployment of resources across different environments. 

## tldr 
 
> Manage marketplace agreement with marketplaceordering.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/term>.

- Print marketplace terms:

`az term show --product "{{product_identifier}}" --plan "{{plan_identifier}}" --publisher "{{publisher_identifier}}"`

- Accept marketplace terms:

`az term accept --product "{{product_identifier}}" --plan "{{plan_identifier}}" --publisher "{{publisher_identifier}}"`
