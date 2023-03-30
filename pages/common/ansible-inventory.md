# ansible-inventory 
## chatgpt 
`ansible-inventory` is a command-line tool in Ansible that generates inventory dynamically. It allows users to get an overview of what hosts and groups are available for their use in various Ansible commands, such as running plays and executing ad-hoc commands.

Here's a brief overview of the most important options for `ansible-inventory`:

- `--list` - prints the current inventory in JSON format
- `--graph` - outputs a visualization of the inventory in graph format
- `--yaml` - selects YAML format rather than JSON
- `--playbook-dir` - specifies the base directory where playbooks are located
- `--inventory` - specifies the location of the inventory file
- `--vars` - prints variables for hosts and groups
- `-i` - shorthand for `--inventory`

For example, to list all the hosts and groups used in an Ansible playbook, you can run:

```
ansible-inventory --list --playbook-dir /path/to/playbook
```

This will output information about the inventory in JSON format. You can also visualize the inventory by running:

```
ansible-inventory --graph
```

This will produce a graphical representation of the inventory, highlighting the relationships between hosts and groups. Other options can be used to extract specific information about the inventory, such as variables or certain groups of hosts. 

## tldr 
 
> Display or dump an Ansible inventory.
> See also: `ansible`.
> More information: <https://docs.ansible.com/ansible/latest/cli/ansible-inventory.html>.

- Display the default inventory:

`ansible-inventory --list`

- Display a custom inventory:

`ansbile-inventory --list --inventory {{path/to/file_or_script_or_directory}}`

- Display the default inventory in YAML:

`ansible-inventory --list --yaml`

- Dump the default inventory to a file:

`ansible-inventory --list --output {{path/to/file}}`
