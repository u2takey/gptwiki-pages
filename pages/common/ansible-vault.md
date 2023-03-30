# ansible-vault 
## chatgpt 
Ansible-vault is a command-line tool that allows you to create and manage encrypted files containing sensitive data used by Ansible's playbooks or tasks. The purpose of this tool is to enable secure storage of essential information such as passwords, API keys, and other secret data that is required for the deployment or management of infrastructure using Ansible.

The tool provides three primary command-line options:

1. Create: This subcommand allows you to create a new encrypted file. You can use this option to initialize the password or change it after creation. The syntax for creating a new encrypted file is as follows:

   ```
   ansible-vault create <filename>
   ```

2. Edit: This subcommand allows you to edit the contents of an encrypted file. The encrypted file must be decrypted first before you can edit it. The syntax for editing an encrypted file is as follows:

   ```
   ansible-vault edit <filename>
   ```

3. View: This subcommand allows you to view the contents of an encrypted file without decrypting it. This option does not require a password. The syntax to view the contents of an encrypted file is as follows:

   ```
   ansible-vault view <filename>
   ```

The tool also provides several other subcommands, including encrypt, decrypt, and rekey, which allows you to encrypt, decrypt, or change the password of an encrypted file, respectively. Overall, the ansible-vault command-line tool is a powerful feature that helps developers to safely manage and protect the sensitive credentials and information stored in files used by Ansible. 

## tldr 
 
> Encrypts & decrypts values, data structures and files within Ansible projects.
> More information: <https://docs.ansible.com/ansible/latest/user_guide/vault.html#id17>.

- Create a new encrypted vault file with a prompt for a password:

`ansible-vault create {{vault_file}}`

- Create a new encrypted vault file using a vault key file to encrypt it:

`ansible-vault create --vault-password-file={{password_file}} {{vault_file}}`

- Encrypt an existing file using an optional password file:

`ansible-vault encrypt --vault-password-file={{password_file}} {{vault_file}}`

- Encrypt a string using Ansible's encrypted string format, displaying interactive prompts:

`ansible-vault encrypt_string`

- View an encrypted file, using a password file to decrypt:

`ansible-vault view --vault-password-file={{password_file}} {{vault_file}}`

- Re-key already encrypted vault file with a new password file:

`ansible-vault rekey --vault-password-file={{old_password_file}} --new-vault-password-file={{new_password_file}} {{vault_file}}`
