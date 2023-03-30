# puppet apply 
## chatgpt 
Puppet apply is a command used to apply a Puppet manifest immediately, without the need to wait for the next scheduled run. 

In detail, Puppet is a configuration management tool that enables users to automate the process of managing their systems' configurations. A user writes code in the Puppet domain-specific language called Puppet manifests, which describe the desired state of the system. The manifests include information about which packages to install, which files to create or edit, and how to start services or daemons.

When a manifest is created, it needs to be applied to the target system or systems. This is where the puppet apply command comes in. It is used to apply the manifest to the system immediately. The syntax for the command is:

```
puppet apply <manifest>
```

Here, <manifest> is the path to the Puppet manifest that needs to be applied.

When the command is run, Puppet reads the manifest and compares the desired state to the current state of the system. If there are any differences, Puppet makes the necessary changes to the system to bring it to the desired state described in the manifest.

The puppet apply command is useful for testing and applying changes to a system without waiting for the next periodic Puppet run. It is also used in scenarios where a user needs to quickly apply a change to a system, without waiting for Puppet to pick up the changes during the next run. 

## tldr 
 
> Apply Puppet manifests locally.
> More information: <https://puppet.com/docs/puppet/7/man/apply.html>.

- Apply a manifest:

`puppet apply {{path/to/manifest}}`

- Execute puppet code:

`puppet apply --execute {{code}}`

- Use a specific module and hiera config file:

`puppet apply --modulepath {{path/to/directory}} --hiera_config {{path/to/file}} {{path/to/manifest}}`
