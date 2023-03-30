# nixos-option 
## chatgpt 
nixos-option is a command in the NixOS operating system that allows the user to view the available options for a specific attribute or module in NixOS.

The syntax for the nixos-option command is:

```
nixos-option [--description] [--type] [--source] <attribute>
```

This command takes the following parameters:

1. --description: This will display a brief description of the option.

2. --type: This will display the data type of the option.

3. --source: This will display the source location of the option.

4. <attribute>: This is the name of the attribute or module for which you want to view the available options.

For example, if you want to view the available options for the networking module in NixOS, you can use the following command:

```
nixos-option networking
```

This will display a list of all the available options for the networking module, such as network.interfaces, network.enableIPv6, network.defaultGateway, and more.

Overall, the nixos-option command is a helpful tool for exploring the available options in NixOS and learning more about specific attributes and modules. 

## tldr 
 
> Inspect a NixOS configuration.
> More information: <https://nixos.org/manual/nixos/stable/index.html#sec-modularity>.

- List all subkeys of a given option key:

`nixos-option {{option_key}}`

- List current boot kernel modules:

`nixos-option boot.kernelModules`

- List authorized keys for a specific user:

`nixos-option users.users.{{username}}.openssh.authorizedKeys.{{keyFiles|keys}}`

- List all remote builders:

`nixos-option nix.buildMachines`

- List all subkeys of a given key on another NixOS configuration:

`NIXOS_CONFIG={{path_to_configuration.nix}} nixos-option {{option_key}}`

- Show recursively all values of a user:

`nixos-option -r users.users.{{user}}`
