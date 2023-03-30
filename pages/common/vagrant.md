# vagrant 
## chatgpt 
Vagrant is a command-line tool that is used to create, configure, and manage virtual machines. The tool uses a configuration file called Vagrantfile to specify the settings needed for the virtual machine. When you execute a command that starts with "vagrant", you will be configuring or managing a virtual machine using the Vagrant tool.

Here are some common Vagrant commands and what they do:

- `vagrant init`: This command creates a new Vagrantfile in the current directory. The file will contain default settings for a virtual machine.
- `vagrant up`: This command starts a new virtual machine based on the settings specified in the Vagrantfile. If the virtual machine does not exist yet, it will be created. If it already exists, it will be started.
- `vagrant ssh`: This command connects to the virtual machine via SSH. It is a convenient way to access the virtual machine's console without having to use a GUI interface.
- `vagrant halt`: This command stops the virtual machine. It is equivalent to shutting down a physical computer.
- `vagrant destroy`: This command deletes the virtual machine and all its associated resources. This is useful if you want to start over with a clean slate.

Overall, Vagrant is a powerful tool that helps developers and IT professionals manage virtual machines with ease. It simplifies the process of creating, configuring, and managing virtual machines, making it a great choice for those who need to work with virtual machines frequently. 

## tldr 
 
> Manage lightweight, reproducible, and portable development environments.
> More information: <https://www.vagrantup.com>.

- Create Vagrantfile in current directory with the base Vagrant box:

`vagrant init`

- Create Vagrantfile with the Ubuntu 20.04 (Focal Fossa) box from HashiCorp Atlas:

`vagrant init ubuntu/focal64`

- Start and provision the vagrant environment:

`vagrant up`

- Suspend the machine:

`vagrant suspend`

- Halt the machine:

`vagrant halt`

- Connect to machine via SSH:

`vagrant ssh`

- Output the SSH configuration file of the running Vagrant machine:

`vagrant ssh-config`

- List all local boxes:

`vagrant box list`
