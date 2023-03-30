# consul-kv 
## chatgpt 
Consul is a distributed service mesh that is used for service networking and discovery, as well as service segmentation and routing. One of its key features is its Key/Value (KV) store which is a flexible and powerful storage mechanism that can be used to store configuration data, metadata, and other information.

The `consul-kv` command is a tool that is used to interact with the Consul KV store. It allows users to store and retrieve data from the KV store using the command line interface, making it easy to automate interactions with the store.

Some common uses of the `consul-kv` command include setting and getting configuration values for applications, storing metadata about services, and storing custom data that can be used by Consul's other features such as health checks and service discovery.

To use the `consul-kv` command, users must have access to a Consul cluster and be authorized to interact with the KV store. The command can be used with various flags and arguments to specify the key and value to be stored or retrieved, as well as other configuration options such as setting TTLs and modifying ACLs. 

## tldr 
 
> Distributed key-value store with health checking and service discovery.
> More information: <https://learn.hashicorp.com/consul/getting-started/kv>.

- Read a value from the key-value store:

`consul kv get {{key}}`

- Store a new key-value pair:

`consul kv put {{key}} {{value}}`

- Delete a key-value pair:

`consul kv delete {{key}}`
