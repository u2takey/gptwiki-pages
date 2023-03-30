# keyctl 
## chatgpt 
`keyctl` is a command-line interface for managing the Linux kernel key management facility. It allows users and applications to create, manipulate, and destroy cryptographic keys and security tokens. 

Some of the most commonly used commands with `keyctl` include:

- `add`: Adds a new key to the kernel keyring. You can specify the type of key (e.g. symmetric, asymmetric, or certificate), the key's description, and the key's payload (e.g. the key value or certificate).
- `link`: Links a key to another key, creating a keyring hierarchy. This can be useful for organizing keys, as you can create 'sub-keyrings' within the main keyring.
- `search`: Searches for a key in the keyring, based on its description or type.
- `unlink`: Unlinks a key from its parent keyring.
- `describe`: Prints information about a key, such as its description, type, and payload.
- `revoke`: Revokes a key, rendering it unusable. This is often done when a key is compromised or no longer needed.

The `keyctl` command can be used by both users and system administrators, typically through a terminal or shell. It is often used in conjunction with other security-related commands, such as `openssl`, to manage and secure cryptographic keys and certificates. 

## tldr 
 
> Manipulate the Linux kernel keyring.
> More information: <https://manned.org/keyctl>.

- List keys in a specific keyring:

`keyctl list {{target_keyring}}`

- List current keys in the user default session:

`keyctl list {{@us}}`

- Store a key in a specific keyring:

`keyctl add {{type_keyring}} {{key_name}} {{key_value}} {{target_keyring}}`

- Store a key with its value from standard input:

`echo -n {{key_value}} | keyctl padd {{type_keyring}} {{key_name}} {{target_keyring}}`

- Put a timeout on a key:

`keyctl timeout {{key_name}} {{timeout_in_seconds}}`

- Read a key and format it as a hex-dump if not printable:

`keyctl read {{key_name}}`

- Read a key and format as-is:

`keyctl pipe {{key_name}}`

- Revoke a key and prevent any further action on it:

`keyctl revoke {{key_name}}`
