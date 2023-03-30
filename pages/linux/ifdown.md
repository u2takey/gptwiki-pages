# ifdown 
## chatgpt 
The "ifdown" command on a Linux or Unix system is used to shut down a network interface. 

When executed, the command triggers the system to release any settings and resources associated with the specified interface, including its IP address and routing information. 

To use the command, you must specify the name of the interface you wish to bring down. For example, "ifdown eth0" would shut down the network interface named "eth0". 

This command is typically used in networking scripts or in terminal when troubleshooting network connectivity issues. It is important to note that using this command will disconnect the interface from the network, and any data being transmitted or received through the interface may be lost. 

## tldr 
 
> Disable network interfaces.
> More information: <https://manned.org/ifdown>.

- Disable interface eth0:

`ifdown {{eth0}}`

- Disable all interfaces which are enabled:

`ifdown -a`
