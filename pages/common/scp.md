# scp 
## chatgpt 
The scp (secure copy) command is used in Linux and Unix-based operating systems to securely transfer files between local and remote computers over a network. It is a fast and secure alternative to FTP (File Transfer Protocol).

Syntax:
scp [options] [source_file] [destination]

Options:
- P: specify port number
- r: recursive copying of directories and their contents
- p: preserve permissions and timestamps of the files being copied
- v: verbose mode, provides detailed output of the transfer process
- q: quiet mode, suppresses all output except for errors
- C: enable compression during transfer
- i: specifies the identity file (private key) for authentication

Source File: The file or set of files to be copied. It can be specified by a relative or absolute path.

Destination: The destination where the source file will be copied. It can be a directory or a filename.

Examples:
To copy a file from a local system to a remote system at IP address 192.168.1.10:
```
scp file.txt user@192.168.1.10:/home/user/
```

To copy a file from a remote system to a local system:
```
scp user@192.168.1.10:/home/user/file.txt /home/user/
```

To copy files recursively and preserve their permissions:
```
scp -rp /home/user/folder user@192.168.1.10:/home/user/
```

To copy a file using a specified port number:
```
scp -P 2222 file.txt user@192.168.1.10:/home/user/
```

To use a private key for authentication:
```
scp -i /path/to/key.pem file.txt user@192.168.1.10:/home/user/
``` 

## tldr 
 
> Secure copy.
> Copy files between hosts using Secure Copy Protocol over SSH.
> More information: <https://man.openbsd.org/scp>.

- Copy a local file to a remote host:

`scp {{path/to/local_file}} {{remote_host}}:{{path/to/remote_file}}`

- Use a specific port when connecting to the remote host:

`scp -P {{port}} {{path/to/local_file}} {{remote_host}}:{{path/to/remote_file}}`

- Copy a file from a remote host to a local directory:

`scp {{remote_host}}:{{path/to/remote_file}} {{path/to/local_directory}}`

- Recursively copy the contents of a directory from a remote host to a local directory:

`scp -r {{remote_host}}:{{path/to/remote_directory}} {{path/to/local_directory}}`

- Copy a file between two remote hosts transferring through the local host:

`scp -3 {{host1}}:{{path/to/remote_file}} {{host2}}:{{path/to/remote_directory}}`

- Use a specific username when connecting to the remote host:

`scp {{path/to/local_file}} {{remote_username}}@{{remote_host}}:{{path/to/remote_directory}}`

- Use a specific ssh private key for authentication with the remote host:

`scp -i {{~/.ssh/private_key}} {{local_file}} {{remote_host}}:{{/path/remote_file}}`
