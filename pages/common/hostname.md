# hostname 
## chatgpt 
The command "hostname" is a simple command that is used to check or set the host name of a Unix-based system. When you run the hostname command without any options, it will display the current hostname of the system. 

Here’s an example:

$ hostname
my.hostname.com

If you want to set a new hostname, you can use the -s option followed by the new hostname. You need to have administrator privileges to set a new hostname.

Here’s an example:

$ sudo hostname -s new.hostname.com

The hostname command is helpful when you need to identify the name of the system you are working on or when you want to change the name of the system. The hostname is also used for network communication and can help identify a system on the network. 

## tldr 
 
> Show or set the system's host name.
> More information: <https://manned.org/hostname>.

- Show current host name:

`hostname`

- Show the network address of the host name:

`hostname -i`

- Show all network addresses of the host:

`hostname -I`

- Show the FQDN (Fully Qualified Domain Name):

`hostname --fqdn`

- Set current host name:

`hostname {{new_hostname}}`
