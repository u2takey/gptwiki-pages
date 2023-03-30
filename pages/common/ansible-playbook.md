# ansible-playbook 
## chatgpt 
The `ansible-playbook` command is used to execute an Ansible playbook. A playbook is a collection of tasks that are executed against one or more remote hosts. The `ansible-playbook` command takes the following form:

```
ansible-playbook playbook-file.yml
```

where `playbook-file.yml` is the name of the file that contains the playbook.

Here are some of the key options that can be used with the `ansible-playbook` command:

- `-i, --inventory`: Specifies the inventory file that should be used to define the hosts that the playbook will be executed against.
- `-l, --limit`: Specifies the subset of hosts from the inventory that the playbook should be executed against. This can be used to limit the playbook to a specific subset of hosts.
- `-e, --extra-vars`: Allows you to specify extra variables that will be available to the playbook. These variables can be used to customize the behavior of the playbook.
- `-t, --tags`: Specifies a subset of tasks within the playbook that should be executed. This can be used to execute specific tasks within a playbook.
- `--check`: The `--check` flag tells Ansible to perform a "dry run" of the playbook, without actually executing any tasks. This can be useful to verify that the playbook will have the expected effect.

The `ansible-playbook` command is a powerful tool for automating complex tasks on remote hosts, and is a key part of the Ansible toolset. 

## tldr 
 
> Execute tasks defined in playbook on remote machines over SSH.
> More information: <https://docs.ansible.com/ansible/latest/cli/ansible-playbook.html>.

- Run tasks in playbook:

`ansible-playbook {{playbook}}`

- Run tasks in playbook with custom host inventory:

`ansible-playbook {{playbook}} -i {{inventory_file}}`

- Run tasks in playbook with extra variables defined via the command-line:

`ansible-playbook {{playbook}} -e "{{variable1}}={{value1}} {{variable2}}={{value2}}"`

- Run tasks in playbook with extra variables defined in a JSON file:

`ansible-playbook {{playbook}} -e "@{{variables.json}}"`

- Run tasks in playbook for the given tags:

`ansible-playbook {{playbook}} --tags {{tag1,tag2}}`

- Run tasks in a playbook starting at a specific task:

`ansible-playbook {{playbook}} --start-at {{task_name}}`
