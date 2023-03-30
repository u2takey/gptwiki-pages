# smbmap 
## chatgpt 
The 'smbmap' command is a utility tool used to scan SMB (Server Message Block) shares on a network or host to find out which ones are available and accessible to the user who is running the command. SMB is a network protocol that allows file sharing, printer sharing, and communication between network devices.

The smbmap command can be used to:

1. Authenticate on SMB shares - Use the '-u' and '-p' options to pass the username and password for the authentication.

2. List available shares - Use the '-H' option to specify the target host or IP address, and the '-R' option to specify if you want to recursively list subdirectories.

3. Show share permissions - Use the '-H' option to specify the target host or IP address and the '-s' option to specify the name of the share.

4. Map remote share directories locally - Use the '-H' option to specify the target host or IP address, the '-s' option to specify the name of the share and the '-d' option to specify the directory or file you want to download.

Example usage:

1. Authenticate on SMB shares: smbmap -H 192.168.1.100 -u user -p password.

2. List available shares: smbmap -H 192.168.1.100 -R.

3. Show share permissions: smbmap -H 192.168.1.100 -s sharename.

4. Map remote share directories locally: smbmap -H 192.168.1.100 -u user -p password -s sharename -d remotefile localfile. 

## tldr 
 
> SMB enumeration tool.
> More information: <https://github.com/ShawnDEvans/smbmap>.

- Display SMB shares and permissions on a host, prompting for user's password or NTLM hash:

`smbmap -u {{username}} --prompt -H {{ip}}`

- Display SMB shares and permissions on a host, specifying the domain and passing the password NTLM hash:

`smbmap -u {{username}} --prompt -d {{domain}} -H {{ip}}`

- Display SMB shares and list a single level of directories and files:

`smbmap -u {{username}} --prompt -H {{ip}} -r`

- Display SMB shares and recursively list a defined number of levels of directories and files:

`smbmap -u {{username}} --prompt -H {{ip}} -R --depth {{3}}`

- Display SMB shares and recursively list directories and files, downloading the files matching a regular expression:

`smbmap -u {{username}} --prompt -H {{ip}} -R -A {{pattern}}`

- Display SMB shares and recursively list directories and files, searching for file content matching a regular expression:

`smbmap -u {{username}} --prompt -H {{ip}} -R -F {{pattern}}`

- Execute a shell command on a remote system:

`smbmap -u {{username}} --prompt -H {{ip}} -x {{command}}`

- Upload a file to a remote system:

`smbmap -u {{username}} --prompt -H {{ip}} --upload {{source}} {{destination}}`
