# nmblookup 
## chatgpt 
nmblookup is a command-line tool used in Linux and UNIX-based operating systems to query NetBIOS over TCP/IP (NBT) and lookup NetBIOS names. NetBIOS is a protocol used by Windows-based systems to allow computers to communicate on a local area network (LAN).

The nmblookup command allows a user to retrieve information about the NetBIOS names of computers on the network. It can be used to:

- Resolve a NetBIOS name to an IP address
- Get information about the NetBIOS name of a computer, such as the domain, workgroup, or server name

The syntax of the nmblookup command is as follows:

nmblookup [options] NetBIOS_name

Here are some of the available options for the nmblookup command:

- -a: Displays the NetBIOS name of a remote machine along with its IP address and MAC address if available.
- -A: Displays the NetBIOS name of a remote machine along with detailed output, including the IP address, MAC address, and workgroup/domain name if available.
- -B: Broadcasts the name query to all computers on the network, not just the ones in the specified subnet.
- -M: Queries the NetBIOS name of a remote machine using the NetBIOS name service instead of the node status query (default).
- -R: Performs a reverse lookup of an IP address to find the corresponding NetBIOS name.

Here's an example of how to use the nmblookup command to query a NetBIOS name:

nmblookup -a SMBserver

This command will display the IP address and MAC address of the computer with the NetBIOS name "SMBserver" if it is available on the network. 

## tldr 
 
> Discover SMB shares.
> More information: <https://www.samba.org/samba/docs/current/man-html/nmblookup.1.html>.

- Find hosts in the local network with SMB shares:

`nmblookup -S '*'`

- Find hosts in the local network with SMB shares run by SAMBA:

`nmblookup --status __SAMBA__`
