# etcdctl 
## chatgpt 
`etcdctl` is a command-line client tool for etcd, a distributed key-value store used for storing and retrieving configuration data for distributed systems. The `etcdctl` command allows users to interact with the etcd cluster and manage its data by performing various CRUD (Create, Read, Update and Delete) operations.

Here are some examples of commonly used commands in `etcdctl`:

1. `etcdctl put`: This command is used to store the data in the etcd cluster. It requires a key-value pair to be specified, and the value can be a string, binary or JSON data.

2. `etcdctl get`: This command is used to retrieve the data from the etcd cluster. It requires the key of the data to be specified, and it will return the corresponding value.

3. `etcdctl watch`: This command is used to watch for changes to the data in the etcd cluster. It requires the key of the data to be specified, and it will continuously monitor the key for any changes made to it.

4. `etcdctl del`: This command is used to delete the data from the etcd cluster. It requires the key of the data to be specified, and it will remove the corresponding key-value pair from the etcd cluster.

Other commonly used commands in `etcdctl` include `ls`, `mk`, `rm`, `set`, `update`, and `member`. By using these commands, users can effectively manage and retrieve data from the etcd cluster. 

## tldr 
 
> CLI interface for interacting with etcd, a highly-available key-value pair store.
> More information: <https://etcd.io/docs/latest/dev-guide/interacting_v3/>.

- Display the value associated with a specified key:

`etcdctl get {{my/key}}`

- Store a key-value pair:

`etcdctl put {{my/key}} {{my_value}}`

- Delete a key-value pair:

`etcdctl del {{my/key}}`

- Store a key-value pair, reading the value from a file:

`etcdctl put {{my/file}} < {{path/to/file.txt}}`

- Save a snapshot of the etcd keystore:

`etcdctl snapshot save {{path/to/snapshot.db}}`

- Restore a snapshot of an etcd keystore (restart the etcd server afterwards):

`etcdctl snapshot restore {{path/to/snapshot.db}}`

- Add a user:

`etcdctl user add {{my_user}}`

- Watch a key for changes:

`etcdctl watch {{my/key}}`
