# ssh-add 
## chatgpt 
The ssh-add command is used to add private key identities to the SSH authentication agent. When a user logs in and starts an SSH session, an authentication agent is launched. The authentication agent is responsible for keeping the user's private key(s) in memory so they do not have to be entered each time the user wants to connect to a remote server using SSH.

The ssh-add command is used to add a private key identity to the authentication agent. It can be used with the -l option to list the fingerprints of all identities currently held by the agent, and with the -d option to delete an identity from the agent.

When using ssh-add, the user is prompted to enter the passphrase associated with the private key identity. The passphrase is used to encrypt the private key and protect it from unauthorized access. Once the passphrase is entered, the private key identity is added to the authentication agent and can be used to authenticate the user to remote servers without entering the passphrase again. 

## tldr 
 
> Manage loaded ssh keys in the ssh-agent.
> Ensure that ssh-agent is up and running for the keys to be loaded in it.
> More information: <https://man.openbsd.org/ssh-add>.

- Add the default ssh keys in `~/.ssh` to the ssh-agent:

`ssh-add`

- Add a specific key to the ssh-agent:

`ssh-add {{path/to/private_key}}`

- List fingerprints of currently loaded keys:

`ssh-add -l`

- Delete a key from the ssh-agent:

`ssh-add -d {{path/to/private_key}}`

- Delete all currently loaded keys from the ssh-agent:

`ssh-add -D`

- Add a key to the ssh-agent and the keychain:

`ssh-add -K {{path/to/private_key}}`
