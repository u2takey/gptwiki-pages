# etcd 
## chatgpt 
etcd is a distributed database that stores key-value pairs and makes them accessible to multiple clients. It is designed to provide a reliable and highly-available data store for use in distributed systems.

The etcd command is used to interact with the etcd server. It provides a command-line interface for managing the etcd server and its key-value pairs.

Some examples of etcd command-line options and actions are:

- etcdctl put <key> <value>: This command stores a key-value pair in the etcd server. The <key> and <value> parameters are replaced with the actual key and value that are being stored.

- etcdctl get <key>: This command retrieves the value of a key from the etcd server. The <key> parameter is replaced with the actual key that is being retrieved.

- etcdctl watch <key>: This command watches for changes to a key in the etcd server. If the value of the key changes, the command will display the new value.

- etcdctl cluster-health: This command checks the health of the etcd cluster. It displays information about the cluster's health status, including the number of nodes that are currently online.

Overall, the etcd command is an essential tool for managing a distributed database and ensuring reliable and highly-available data access in a distributed system. 

## tldr 
 
> A distributed, reliable key-value store for the most critical data of a distributed system.
> More information: <https://etcd.io>.

- Start a single-node etcd cluster:

`etcd`

- Start a single-node etcd cluster, listening for client requests on a custom URL:

`etcd --advertise-client-urls {{http://127.0.0.1:1234}} --listen-client-urls {{http://127.0.0.1:1234}}`

- Start a single-node etcd cluster with a custom name:

`etcd --name {{my_etcd_cluster}}`

- Start a single-node etcd cluster with extensive metrics available at http://localhost:2379/debug/pprof/:

`etcd --enable-pprof --metrics extensive`
