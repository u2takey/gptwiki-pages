# az redis 
## chatgpt 
The command "az redis" is a command in the Azure CLI (Command Line Interface) tool that allows you to manage your Azure Redis Cache instance. 

Azure Redis Cache is a fully-managed, in-memory data storage service that provides high throughput, low-latency data access to your applications. Redis (Remote Dictionary Server) is an open-source, in-memory key-value data store that works as a database, cache, and message broker. Azure Redis Cache is built on the open-source Redis database engine, and provides multiple benefits including high availability and scalability. 

The "az redis" command allows you to interact with your Azure Redis Cache instance using the Azure CLI, and perform various operations such as creating, managing, and deleting Redis Cache instances. 

Here are some examples of the operations that you can perform using the "az redis" command:

- Create a new Redis Cache instance: "az redis create"
- List all your Redis Cache instances: "az redis list"
- Get details about a particular Redis Cache instance: "az redis show"
- Update the configuration of a Redis Cache instance: "az redis update"
- Delete a Redis Cache instance: "az redis delete"

The "az redis" command also supports additional options and parameters that allow you to customize and refine your Redis Cache operations based on your specific requirements. 

Overall, the "az redis" command is a powerful tool that allows you to manage your Azure Redis Cache instances easily and efficiently using the command-line interface. 

## tldr 
 
> Manage Redis caches.
> Part of `azure-cli`.
> More information: <https://docs.microsoft.com/cli/azure/redis>.

- Create a new Redis cache instance:

`az redis create --location {{location}} --name {{name}} --resource-group {{resource_group}} --sku {{Basic|Premium|Standard}} --vm-size {{c0|c1|c2|c3|c4|c5|c6|p1|p2|p3|p4|p5}}`

- Update a Redis cache:

`az redis update --name {{name}} --resource-group {{resource_group}} --sku {{Basic|Premium|Standard}} --vm-size {{c0|c1|c2|c3|c4|c5|c6|p1|p2|p3|p4|p5}}`

- Export data stored in a Redis cache:

`az redis export --container {{container}} --file-format {{file-format}} --name {{name}} --prefix {{prefix}} --resource-group {{resource_group}}`

- Delete a Redis cache:

`az redis delete --name {{name}} --resource-group {{resource_group}} --yes`
