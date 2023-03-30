# safe 
## chatgpt 
As an AI language model, I can provide you an overview of the 'safe' command, but the specific details may depend on the platform, operating system, or context in which it is used.

The 'safe' command is generally used to indicate that a program or operation has been completed, and everything is secure or safe. For example, in cryptography, the 'safe' command may mean that a message has been encrypted, and the encryption process has been completed securely without any errors.

In some cases, the 'safe' command may also be used to terminate or interrupt a risky or unsafe operation. For instance, if you are downloading a corrupted file, you can use the 'safe' command to stop the process and prevent further damage to the system.

In other contexts, 'safe' could mean the environment is secure for some activity. For example, you might use the command "python safe.py" to launch a python program that has malware checking steps in place to ensure the environment is free of malicious code.

Overall, the use of the 'safe' command depends on the specific situation, and it can have different meanings based on the context. 

## tldr 
 
> A CLI to interact with HashiCorp Vault.
> More information: <https://github.com/starkandwayne/safe>.

- Add a safe target:

`safe target {{vault_addr}} {{target_name}}`

- Authenticate the CLI client against the Vault server, using an authentication token:

`safe auth {{authentication_token}}`

- Print the environment variables describing the current target:

`safe env`

- Display a tree hierarchy of all reachable keys for a given path:

`safe tree {{path}}`

- Move a secret from one path to another:

`safe move {{old/path/to/secret}} {{new/path/to/secret}}`

- Generate a new 2048-bit SSH key-pair and store it:

`safe ssh {{2048}} {{path/to/secret}}`

- Set non-sensitive keys for a secret:

`safe set {{path/to/secret}} {{key}}={{value}}`

- Set auto-generated password in a secret:

`safe gen {{path/to/secret}} {{key}}`
