# smbmap 
## chatgpt 
The smbmap command is a tool used in Linux and other Unix-like operating systems to scan and explore SMB (Server Message Block) shares on a network. The command is typically used to identify accessible network shares and determine the level of access permissions available to the user. Here are the options available when using the smbmap command:

1. -H: This option specifies the hostname or IP address of the target machine to scan.

2. -u: This specifies the username to use when accessing the shares on the target machine.

3. -p: This specifies the password to use when accessing the shares on the target machine.

4. -d: This option is used to specify the domain name to connect to.

5. -S: This option specifies whether to use SMBv1, SMBv2, or SMBv3 protocol.

6. -P: This option specifies the port number on which to connect to the target machine.

7. -x: This option is used to specify a custom payload for testing vulnerability issues with the target machine.

Once the necessary options are provided, the smbmap command will run a scan of the target machine and provide a list of available network shares along with the level of access permissions available to the user specified in the -u option. With this information, the user can then access the shared files, folders, and resources available on the target machine. 

## tldr 
 
> Allow users to enumerate samba share drives across an entire domain.
> More information: <https://github.com/ShawnDEvans/smbmap>.

- Enumerate hosts with NULL sessions enabled and open shares:

`smbmap --host-file {{path/to/file}}`

- Enumerate hosts and check SMB file permissions:

`smbmap --host-file {{path/to/file}} -u {{username}} -p {{password}} -q`

- Connect to an ip or hostname through smb using a username and password:

`smbmap -u {{username}} -p {{password}} -d {{domain}} -H {{ip_or_hostname}}`

- Locate and download files [R]ecursively up to N levels depth, searching for filename pattern (regex), and excluding certain shares:

`smbmap --host-file {{path/to/file}} -u {{username}} -p {{password}} -q -R --depth {{number}} --exclude {{sharename}} -A {{filepattern}}`

- Upload file through smb using username and password:

`smbmap -u {{username}} -p {{password}} -d {{domain}} -H {{ip_or_hostname}} --upload {{path/to/file}} '{{/share_name/remote_filename}}'`
