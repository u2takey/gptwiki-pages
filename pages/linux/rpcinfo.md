# rpcinfo 
## chatgpt 
rpcinfo is a command-line utility in UNIX and Linux operating systems that allows users to query information about remote procedure call (RPC) services on a network.

The rpcinfo command provides different options that give you various information about the RPC services running on the system. Here are some of the key options of the rpcinfo command:

- `-p`: This option lists out all the RPC services registered on the system. It provides information such as program number, version number, transport protocol, and the port number used by each service.

- `-s`: This option displays the statistics for each RPC service registered on the system. This includes the number of procedure calls made to each service and the number of failures encountered.

- `-u`: This option lists all the registered UDP-based RPC services on the system.

- `-t`: This option displays all the registered TCP-based RPC services on the system.

By default, when the rpcinfo command is executed without any options or arguments, it displays a list of all the RPC services registered on the local system. If you specify a hostname as an argument, it will display the RPC services registered on the specified remote host.

Overall, the rpcinfo command is a useful tool for managing and troubleshooting remote procedure call services on a network. 

## tldr 
 
> Makes an RPC call to an RPC server and reports what it finds.
> More information: <https://manned.org/rpcinfo>.

- Show full table of all RPC services registered on localhost:

`rpcinfo`

- Show concise table of all RPC services registered on localhost:

`rpcinfo -s {{localhost}}`

- Display table of statistics of rpcbind operations on localhost:

`rpcinfo -m`

- Display list of entries of given service name (mountd) and version number (2) on a remote nfs share:

`rpcinfo -l {{remote_nfs_server_ip}} {{mountd}} {{2}}`

- Delete the registration for version 1 of the mountd service for all transports:

`rpcinfo -d {{mountd}} {{1}}`
