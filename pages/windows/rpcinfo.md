# rpcinfo 
## chatgpt 
The rpcinfo command is a utility tool for making RPC (Remote Procedure Call) related queries to an RPC server. RPC is a protocol used to allow a program running on one host to invoke a procedure on a remote host. It uses a client-server model, where the client sends a request to the server and the server responds with the requested information.

The rpcinfo command has several options, including:

- -p: This option provides a list of all the registered RPC services on the specified host.
- -s: This option displays summary information about all the RPC services on the specified host.
- -t: This option shows the transport type used by each RPC service.
- -u: This option displays the universal addresses for each RPC service.
- -d: This option shows the data representation format used by each RPC service.

To use the rpcinfo command, you need to provide the hostname or IP address of the RPC server you want to query. For example, to display a list of all registered RPC services on a server with the IP address 192.168.1.100, you would enter the following command:

rpcinfo -p 192.168.1.100

This would return a list of all the RPC services registered on the specified server, along with their associated program numbers, version numbers, and transport types. 

## tldr 
 
> List programs via RPC on remote computers.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/rpcinfo>.

- List all programs registered on the local computer:

`rpcinfo`

- List all programs registered on a remote computer:

`rpcinfo /p {{computer_name}}`

- Call a specific program on a remote computer using TCP:

`rpcinfo /t {{computer_name}} {{program_name}}`

- Call a specific program on a remote computer using UDP:

`rpcinfo /u {{computer_name}} {{program_name}}`
