# ansible-doc 
## chatgpt 
Ansible-doc is an Ansible command that is used to display documentation for Ansible modules. This command can be used to quickly find information about how to use various Ansible modules and learn about their different parameters.

When you run the "ansible-doc" command followed by the name of a module, it will display information about that module. This information includes a brief description of the module, its parameters, examples of how to use it, and other important details.

For example, if you want to view the documentation of the "yum" module, you can run the following command:

```
ansible-doc yum
```

This will display the documentation for the "yum" module, including how to install packages using yum, how to add/remove repositories, and how to update packages.

Overall, the "ansible-doc" command is a useful tool for learning how to use Ansible modules and enhancing your understanding of Ansible automation. 

## tldr 
 
> Display information on modules installed in Ansible libraries.
> Display a terse listing of plugins and their short descriptions.
> More information: <https://docs.ansible.com/ansible/latest/cli/ansible-doc.html>.

- List available action plugins (modules):

`ansible-doc --list`

- List available plugins of a specific type:

`ansible-doc --type {{become|cache|callback|cliconf|connection|...}} --list`

- Show information about a specific action plugin (module):

`ansible-doc {{plugin_name}}`

- Show information about a plugin with a specific type:

`ansible-doc --type {{become|cache|callback|cliconf|connection|...}} {{plugin_name}}`

- Show the playbook snippet for action plugin (modules):

`ansible-doc --snippet {{plugin_name}}`

- Show information about an action plugin (module) as JSON:

`ansible-doc --json {{plugin_name}}`
