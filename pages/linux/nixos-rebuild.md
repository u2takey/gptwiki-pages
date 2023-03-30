# nixos-rebuild 
## chatgpt 
The `nixos-rebuild` command is used in NixOS, a Linux distribution that uses the Nix package manager. It is used to rebuild the operating system with a different configuration.

When running the `nixos-rebuild` command, you can specify a configuration file or a configuration expression that describes how your NixOS system should be configured. This allows you to customize your system's settings, install software packages, and more.

Here are the steps that `nixos-rebuild` typically follows:

1. It acquires the requested configuration expression or file.
2. It creates a new system image based on the requested configuration.
3. It sets up a boot loader configuration for the new image.
4. It activates the new configuration by rebooting the system.

Overall, the `nixos-rebuild` command is a powerful tool that lets you easily customize your NixOS system and apply those changes with a single command. 

## tldr 
 
> Reconfigure a NixOS machine.
> More information: <https://nixos.org/nixos/manual/#sec-changing-config>.

- Build and switch to the new configuration, making it the boot default:

`sudo nixos-rebuild switch`

- Build and switch to the new configuration, making it the boot default and naming the boot entry:

`sudo nixos-rebuild switch -p {{name}}`

- Build and switch to the new configuration, making it the boot default and installing updates:

`sudo nixos-rebuild switch --upgrade`

- Rollback changes to the configuration, switching to the previous generation:

`sudo nixos-rebuild switch --rollback`

- Build the new configuration and make it the boot default without switching to it:

`sudo nixos-rebuild boot`

- Build and activate the new configuration, but don't make a boot entry (for testing purposes):

`sudo nixos-rebuild test`

- Build the configuration and open it in a virtual machine:

`sudo nixos-rebuild build-vm`
