# az sshkey 
## chatgpt 
As an AI language model, I cannot use CLI or execute commands on machines, but I can explain the concept of "az sshkey" command. 

"az sshkey" is a command-line interface (CLI) command for the Azure Cloud Management portal. It is used to manage and generate SSH public and private key pairs for use with Azure virtual machines. 

When using SSH to connect to an Azure Virtual Machine, SSH keys are used to authenticate the connection, rather than a username and password. The "az sshkey" command can be used to manage these keys, including creating new pairs and viewing the public keys on file for a particular Virtual Machine. 

Here are the steps to generate an SSH key using the "az sshkey" command:

1. Open the Azure Cloud Shell window from the Azure Portal.
2. Type the "az sshkey create" command.
3. Specify the desired key name and choose which encryption algorithm to use.
4. Save the public key and a *.pem file with the private key to a secure location. 

Once you have generated an SSH key, you can use it to connect to an Azure Virtual Machine directly from the Azure Portal or from a terminal on your local device. 

In summary, "az sshkey" is a CLI command used to generate and manage SSH keys for use with Azure Virtual Machines. 

## tldr 
 
> Manage ssh public keys with virtual machines.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/sshkey>.

- Create a new SSH key:

`az sshkey create --name {{name}} --resource-group {{resource_group}}`

- Upload an existing SSH key:

`az sshkey create --name {{name}} --resource-group {{resource_group}} --public-key "{{@path/to/key.pub}}"`

- List all SSH public keys:

`az sshkey list`

- Show information about an SSH public key:

`az sshkey show --name {{name}} --resource-group {{resource_group}}`
