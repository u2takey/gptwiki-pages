# showmount 
## chatgpt 
The "showmount" command is used in the Linux/Unix operating system to display which NFS (Network File System) exports are currently available from an NFS server. The command lists the names of the file systems that are shared by the server and the client machines that have mounted these file systems. It provides information about the shared file systems and their corresponding mount points, so that clients can access the shared resources on the server. 

When you execute the "showmount" command without any options, it displays a list of all the file systems shared by the NFS server, along with the host names of the systems that have mounted them. The output is presented in a tabular format that includes the file system name, the mount point name, and the list of allowed hosts that can access the shared file system. 

Syntax: showmount [-adehv] [server]

Options:
- a: Shows all the shared file systems, including those that are currently unused or inactive.
- d: Shows the directories that are being used by the client.
- e: Shows a list of all the export definitions on the server.
- h: Shows a brief summary of the available options.
- v: Shows verbose output, which provides more detailed information about the shared file systems.

You can combine different options with the "showmount" command to refine the search results based on your requirements. For example, to list all the active directories on the server that are being used by clients, you can use the command "showmount -d server". 

In summary, the "showmount" command is a useful utility in Linux/Unix that helps to identify the shared file systems on an NFS server and provides information about the mounted directories by the clients. It helps system administrators to manage their network file systems more efficiently by displaying the necessary details about the NFS exports. 

## tldr 
 
> Display information about NFS filesystems on Windows Server.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/showmount>.

- Display all exported filesystems:

`showmount -e`

- Display all NFS clients and their mounted directories:

`showmount -a`

- Display all NFS mounted directories:

`showmount -d`

- Display all exported filesystems for a remote server:

`showmount -e {{server_address}}`
