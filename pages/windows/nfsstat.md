# nfsstat 
## chatgpt 
The "nfsstat" command is a tool commonly used in Linux operating systems that displays various statistics and information about the Network File System (NFS). The command provides a comprehensive overview of NFS-related activities and operations, including the type of requests made, response times, errors encountered, mounts, and file system statistics.

When executed, the "nfsstat" command outputs detailed information on server and client hosts about the status of NFS performance and utilization. It displays the following:

1. Server and client statistics: Provides information about the NFS server and client statistics, including read/write operations, file locking, and file caching.

2. Server and client connections: Displays information about the current connections established between NFS servers and clients.

3. Server and client caching: Shows information about the file system cache on the NFS server and client sides.

4. Command options: The "nfsstat" command also provides several command-line options to customize the output, such as enabling or disabling the display of specific NFS-related statistics, such as retransmitted packets or dropped requests.

Overall, the "nfsstat" command helps system administrators to monitor and troubleshoot performance issues within the NFS infrastructure, allowing them to identify and resolve problems before they cause significant downtime or impact system stability. 

## tldr 
 
> Display or reset the number of calls made to the NFS server.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/nfsstat>.

- Display the recorded number of calls made to the NFS server:

`nfsstat`

- Reset the recorded number of calls made to the NFS server:

`nfsstat -z`
