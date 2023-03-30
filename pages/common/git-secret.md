# git secret 
## chatgpt 
The command "git secret" is a plugin that allows you to encrypt sensitive files within your Git repository. 

When you run "git secret init", it creates a key pair for encryption/decryption and adds the public key to the Git repository. 

Then, when you want to encrypt a file, you run "git secret add [file_path]" which will add the file to a file called ".gitsecret/paths/mapping.cfg" and encrypt the file using the public key. 

You can then push the encrypted file to the remote repository, and only people with the private key can decrypt and view the contents of the file.

When you want to decrypt a file, you run "git secret reveal [file_path]" which will decrypt the specified file using the private key.

The "git secret" command is particularly useful for encrypting files containing passwords, sensitive user data, or proprietary code that you don't want to share with anyone who isn't authorized to see it. 

## tldr 
 
> Bash tool which stores private data inside a Git repository.
> More information: <https://github.com/sobolevn/git-secret>.

- Initialize `git-secret` in a local repository:

`git secret init`

- Grant access to the current Git user's email:

`git secret tell -m`

- Grant access by email:

`git secret tell {{email}}`

- Revoke access by email:

`git secret killperson {{email}}`

- List emails with access to secrets:

`git secret whoknows`

- Register a secret file:

`git secret add {{path/to/file}}`

- Encrypt secrets:

`git secret hide`

- Decrypt secret files:

`git secret reveal`
