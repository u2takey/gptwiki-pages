# salt-key 
## chatgpt 
The 'salt-key' command is a tool that is part of the SaltStack infrastructure automation framework. It is used for managing Salt Minion keys, which are the security certificates that allow a Salt Master to securely communicate with Salt Minions.

When a Salt Minion is first installed, it generates a public and private keypair. The public key is sent to the Salt Master and the private key is kept on the Minion. When the Minion tries to connect to the Master, the Master checks its list of authorized keys to see if the Minion is allowed to communicate with it. If the key has not been authorized yet, the 'salt-key' command can be used to manage the key.

Some common 'salt-key' commands include:

- 'salt-key --list all': This lists all the keys that have been sent to the Salt Master, whether they have been accepted or not.
- 'salt-key --list accepted': This shows a list of all the Minion keys that have been accepted by the Salt Master and are allowed to communicate with it.
- 'salt-key --list rejected': This shows a list of all the Minion keys that have been rejected by the Salt Master and are not allowed to communicate with it.
- 'salt-key --accept=hostname': This accepts the public key for a specific Minion and adds it to the list of authorized keys.
- 'salt-key --delete=hostname': This deletes the key for a specific Minion, which prevents it from connecting to the Salt Master until a new key is generated.

Overall, the 'salt-key' command is a crucial tool for managing the security of your SaltStack infrastructure by controlling which Minions are allowed to communicate with the Salt Master. 

## tldr 
 
> Manages salt minion keys on the salt master.
> Needs to be run on the salt master, likely as root or with sudo.
> More information: <https://docs.saltstack.com/ref/cli/salt-key.html>.

- List all accepted, unaccepted and rejected minion keys:

`salt-key -L`

- Accept a minion key by name:

`salt-key -a {{MINION_ID}}`

- Reject a minion key by name:

`salt-key -r {{MINION_ID}}`

- Print fingerprints of all public keys:

`salt-key -F`
