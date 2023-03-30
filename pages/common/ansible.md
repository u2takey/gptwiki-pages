# ansible 
## chatgpt 
Ansible is an open-source automation tool that is used for managing the configuration, deployment, and orchestration of computer systems. It is written in Python and uses a simple syntax called YAML for describing the configuration policies.

The "ansible" command is the main command used to run Ansible playbooks, which are YAML files that describe a series of tasks to be executed on remote hosts. When running the "ansible" command, you can specify the inventory of hosts to target, the tasks to be executed, and any options or variables to configure the execution.

For example, the basic syntax for running the "ansible" command is:

```
ansible [options] [-i inventory] hosts -m module [-a 'module arguments']
```

Here are some of the important options and arguments that can be used with the "ansible" command:

- "-i inventory": specifies the inventory file that contains a list of hosts to target.
- "-m module": specifies the module to be executed on the remote host. Modules are pre-defined tasks that perform specific actions such as copying files, installing packages, or starting services.
- "-a 'module arguments'": specifies the arguments to be passed to the module.
- "--become": tells Ansible to use privileged escalation (e.g. sudo) when executing tasks on the remote host.
- "-k": prompts the user for the SSH password to authenticate with the remote host.
- "-u username": specifies the username to authenticate with the remote host.

Once the "ansible" command is executed, Ansible will connect to each of the specified hosts and execute the tasks defined in the playbook. The output of the command will show the status and results of each task on each host. 

## tldr 
 
> Manage groups of computers remotely over SSH. (use the `/etc/ansible/hosts` file to add new groups/hosts).
> Some subcommands such as `ansible galaxy` have their own usage documentation.
> More information: <https://www.ansible.com/>.

- List hosts belonging to a group:

`ansible {{group}} --list-hosts`

- Ping a group of hosts by invoking the ping module:

`ansible {{group}} -m ping`

- Display facts about a group of hosts by invoking the setup module:

`ansible {{group}} -m setup`

- Execute a command on a group of hosts by invoking command module with arguments:

`ansible {{group}} -m command -a '{{my_command}}'`

- Execute a command with administrative privileges:

`ansible {{group}} --become --ask-become-pass -m command -a '{{my_command}}'`

- Execute a command using a custom inventory file:

`ansible {{group}} -i {{inventory_file}} -m command -a '{{my_command}}'`

- List the groups in an inventory:

`ansible localhost -m debug -a '{{var=groups.keys()}}'`
