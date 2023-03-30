# ssh-keyscan 
## chatgpt 
The `ssh-keyscan` command is used to retrieve the public key of a remote server and add it to the local user's `known_hosts` file. 

The syntax for the command is: 

```
ssh-keyscan [options] hostname
```

`hostname` specifies the remote server whose public key is to be scanned. The command will connect to the server and retrieve its public key. 

There are several options that can be used with `ssh-keyscan`. Some commonly used options are: 

- `-t <type>`: Specifies the type of key to retrieve. Possible values are `rsa`, `dsa`, `ecdsa`, and `ed25519`. By default, all available key types are retrieved. 
- `-p <port>`: Specifies the port number to use for the SSH connection. By default, port 22 is used. 
- `-f <filename>`: Specifies the file to which the retrieved keys should be written. By default, the keys are added to the `known_hosts` file in the user's home directory. 
- `-H`: This option is used to hash the hostnames and IP addresses in the output. 

Once the public key is retrieved, it is added to the `known_hosts` file on the local machine. This allows the user to connect to the remote server without being prompted to verify the server's identity every time they connect. 

Overall, the `ssh-keyscan` command is a useful tool for automating the process of adding a server's public key to the local `known_hosts` file. 

## tldr 
 
> Get the public ssh keys of remote hosts.
> More information: <https://man.openbsd.org/ssh-keyscan>.

- Retrieve all public ssh keys of a remote host:

`ssh-keyscan {{host}}`

- Retrieve all public ssh keys of a remote host listening on a specific port:

`ssh-keyscan -p {{port}} {{host}}`

- Retrieve certain types of public ssh keys of a remote host:

`ssh-keyscan -t {{rsa,dsa,ecdsa,ed25519}} {{host}}`

- Manually update the ssh known_hosts file with the fingerprint of a given host:

`ssh-keyscan -H {{host}} >> ~/.ssh/known_hosts`
