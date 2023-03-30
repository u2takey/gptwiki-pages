# multipass 
## chatgpt 
Multipass is a command-line utility that allows users to manage and launch virtual machines (VMs) on their local machine. The command provides a simple and efficient way to create and manage VMs in a multi-cloud environment.

Here are some of the most common uses of the multipass command:

1. Creating a VM: The `multipass launch` command is used to create a new VM. Users can specify the number of CPUs, amount of RAM, and disk image size during the creation process.

2. Starting and stopping a VM: The `multipass start` and `multipass stop` commands are used to respectively start and stop a VM.

3. Viewing VM details: The `multipass info` command is used to view detailed information about a running VM, including its IP address and disk space usage.

4. Connecting to a VM: The `multipass shell` command is used to connect to a running VM’s terminal.

5. Managing VM snapshots: The `multipass snapshot` command is used to create, list, and delete snapshots of a VM. Snapshots are useful for saving the state of a VM at a particular point in time.

Overall, the multipass command simplifies the process of managing VMs and enables developers to quickly and easily launch and test different environments. 

## tldr 
 
> CLI to manage Ubuntu virtual machines using native hypervisors.
> More information: <https://multipass.run/>.

- List the aliases that can be used to launch an instance:

`multipass find`

- Launch a new instance, set its name and use a cloud-init configuration file:

`multipass launch -n {{instance_name}} --cloud-init {{configuration_file}}`

- List all the created instances and some of their properties:

`multipass list`

- Start a specific instance by name:

`multipass start {{instance_name}}`

- Show the properties of an instance:

`multipass info {{instance_name}}`

- Open a shell prompt on a specific instance by name:

`multipass shell {{instance_name}}`

- Delete an instance by name:

`multipass delete {{instance_name}}`

- Mount a directory into a specific instance:

`multipass mount {{path/to/local/directory}} {{instance_name}}:{{path/to/target/directory}}`
