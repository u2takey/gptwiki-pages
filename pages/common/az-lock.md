# az lock 
## chatgpt 
The `az lock` command is used in Azure CLI (Command Line Interface) and it is used to create, delete, show, and update the management locks on Azure resources. 

Azure resource locks are used to prevent accidental deletion or modification of critical resources in an Azure subscription. Once a lock is applied to a resource, it prevents the resource and its setters from being deleted, updated or modified.

The syntax of using the command is as follows:

```
az lock {create | delete | show | update}
         [--ids]
         [--name]
         [--namespace]
         [--resource]
         [--resource-group]
         [--notes]
         [--lock-type {ReadOnly | CanNotDelete}]
         [--parent]
```

Here is what each option means:

- `create`: creates a new lock on the specified resource.
- `delete`: deletes a previously created lock from the specified resource.
- `show`: displays details of the lock on the specified resource.
- `update`: modifies the properties of a lock on the specified resource.

- `--ids`: The resource IDs of one or more resources to create a lock for separated by spaces.
- `--name`: The name of the lock.
- `--namespace`: The Microsoft.Insights namespace used for Microsoft.Insights components.
- `--resource`: The resource name to create a lock for (up to maximum of 1600 characters).
- `--resource-group`: Name of the resource group that contains the resource to lock.
- `--notes`: Notes associated with the lock on the resource.
- `--lock-type`: The type of lock to apply on the resource. ReadOnly or CanNotDelete are the options.
- `--parent`: The full path of the parent resource, associated with resources that are created within a resource group. 

In summary, the `az lock` command is a useful tool to prevent unwanted changes or deletions to critical resources in an Azure subscription, and it helps to ensure the safety and security of the resources. 

## tldr 
 
> Manage Azure locks.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/lock>.

- Create a read-only subscription level lock:

`az lock create --name {{lock_name}} --lock-type ReadOnly`

- Create a read-only resource group level lock:

`az lock create --name {{lock_name}} --resource-group {{group_name}} --lock-type ReadOnly`

- Delete a subscription level lock:

`az lock delete --name {{lock_name}}`

- Delete a resource group level lock:

`az lock delete --name {{lock_name}} --resource-group {{group_name}}`

- List out all locks on the subscription level:

`az lock list`

- Show a subscription level lock:

`az lock show -n {{lock_name}}`
