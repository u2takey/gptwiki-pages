# az tag 
## chatgpt 
The "az tag" command is a command-line interface (CLI) command used in Microsoft Azure to manage tags, which are key-value pairs that can be used to organize resources in Azure. 

The basic syntax of the command is: 

az tag {create | delete | list | update | list-values} [OPTIONS] 

The various options available with this command are: 

- create: This option is used to create one or more tags on resources in Azure. You can specify the name of the tag and its value(s) using this option. 

- delete: This option is used to delete one or more tags from resources in Azure. You can specify the name(s) of the tag(s) using this option. 

- list: This option is used to list all the tags applied to resources in Azure. 

- update: This option is used to update the name or value of an existing tag applied to resources in Azure. You can specify the old name of the tag and its new name/value using this option. 

- list-values: This option is used to list all the distinct tag values applied to resources in Azure. 

Overall, the "az tag" command is a useful tool in managing resources in Azure by providing a way to organize them using key-value pairs (tags). 

## tldr 
 
> Manage tags on a resource.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/tag>.

- Create a tag value:

`az tag add-value --name {{tag_name}} --value {{tag_value}}`

- Create a tag in the subscription:

`az tag create --name {{tag_name}}`

- Delete a tag from the subscription:

`az tag delete --name {{tag_name}}`

- List all tags on a subscription:

`az tag list --resource-id /subscriptions/{{subscription_id}}`

- Delete a tag value for a specific tag name:

`az tag remove-value --name {{tag_name}} --value {{tag_value}}`
