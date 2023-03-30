# nixos-container 
## chatgpt 
The "nixos-container" command is used to manage containers in the NixOS operating system. NixOS is a Linux distribution that uses a unique package manager called "Nix" to provide a declarative approach to system configuration.

Containers are lightweight virtual environments that allow for isolated applications and services to run on a single host machine. The "nixos-container" command facilitates the creation, management, and destruction of these containers within the NixOS environment.

The command has several subcommands that allow you to perform different actions such as listing available containers, creating new ones, and starting or stopping them. 

For example, the "nixos-container create" command can be used to create a new container, and the "nixos-container list" command can be used to display a list of all containers currently running.

Overall, the "nixos-container" command is a powerful tool for managing containers in NixOS, providing a simple and efficient way to build and deploy isolated applications and services. 

## tldr 
 
> Starts NixOS containers using Linux containers.
> More information: <https://nixos.org/manual/nixos/stable/#ch-containers>.

- List running containers:

`sudo nixos-container list`

- Create a NixOS container with a specific configuration file:

`sudo nixos-container create {{container_name}} --config-file {{nix_config_file_path}}`

- Start, stop, terminate, or destroy a specific container:

`sudo nixos-container {{start|stop|terminate|destroy|status}} {{container_name}}`

- Run a command in a running container:

`sudo nixos-container run {{container_name}} -- {{command}} {{command_arguments}}`

- Update a container configuration:

`sudo $EDITOR /var/lib/container/{{container_name}}/etc/nixos/configuration.nix && sudo nixos-container update {{container_name}}`

- Enter an interactive shell session on an already-running container:

`sudo nixos-container root-login {{container_name}}`
