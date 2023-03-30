# ssh-keygen 
## chatgpt 
The `ssh-keygen` command is used to generate a new SSH key pair, consisting of a private key and a public key. This command is typically used in a terminal or command prompt environment.

When executed, `ssh-keygen` will prompt the user for some basic settings such as the file name and location for the keys, as well as the type and strength of the encryption to be used. Once these settings have been chosen, `ssh-keygen` will generate the private and public keys and save them to the specified file location.

The private key is used for authentication purposes when connecting to a remote server via SSH. It should be kept secret and never shared, as it provides access to the user's account on the remote server. The public key, on the other hand, can be freely shared with others and is used to verify the user's identity when connecting to a server.

Generated SSH keys are typically stored in the user's home directory in the `.ssh` directory. The private key is saved in a file called `id_rsa` while the corresponding public key is saved in a file called `id_rsa.pub`.

Overall, `ssh-keygen` is a powerful and essential tool for generating secure SSH keys for use in remote server authentication. 

## tldr 
 
> Generate ssh keys used for authentication, password-less logins, and other things.
> More information: <https://man.openbsd.org/ssh-keygen>.

- Generate a key interactively:

`ssh-keygen`

- Specify file in which to save the key:

`ssh-keygen -f {{~/.ssh/filename}}`

- Generate an ed25519 key with 100 key derivation function rounds:

`ssh-keygen -t {{ed25519}} -a {{100}}`

- Generate an RSA 4096-bit key with email as a comment:

`ssh-keygen -t {{dsa|ecdsa|ed25519|rsa}} -b {{4096}} -C "{{comment|email}}"`

- Remove the keys of a host from the known_hosts file (useful when a known host has a new key):

`ssh-keygen -R {{remote_host}}`

- Retrieve the fingerprint of a key in MD5 Hex:

`ssh-keygen -l -E {{md5}} -f {{~/.ssh/filename}}`

- Change the password of a key:

`ssh-keygen -p -f {{~/.ssh/filename}}`

- Change the type of the key format (for example from OPENSSH format to PEM), the file will be rewritten in-place:

`ssh-keygen -p -N "" -m {{PEM}} -f {{~/.ssh/OpenSSH_private_key}}`
