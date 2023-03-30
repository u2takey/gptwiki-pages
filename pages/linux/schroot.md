# schroot 
## chatgpt 
The schroot command is a utility in Linux that is used to run commands or processes in different environments, called chroots. A chroot environment is a restricted environment, separated from the rest of the operating system. The schroot command is commonly used in testing and development environments where different versions of software are required or when isolating potentially harmful or malicious applications.

The basic usage of the schroot command is: 

```
schroot [options] <chroot name> [command]
```

The <chroot name> refers to the name of the chroot environment where the command or process will be run. The [command] argument is optional and, if specified, it is the command or process to be executed in the chroot environment. 

Some common options for the schroot command include:

- -n, --non-interactive: Runs the command in non-interactive mode, without requiring user input.
- -c, --chroot-path: Specifies the path to the chroot directory.
- --userspec: Sets the user and group identity for the executed command.
- -r, --run-session: Runs an interactive shell session in the chroot environment.

In summary, the schroot command is used to execute commands or processes in a chroot environment, which is a separate, restricted environment that isolates the command or process from the rest of the operating system. This is useful for testing and development purposes, as well as for isolating potentially harmful applications. 

## tldr 
 
> Run command or start an interactive shell with a different root directory. More customizable than `chroot`.
> More information: <https://wiki.debian.org/Schroot>.

- Run a command in a specific chroot:

`schroot --chroot {{chroot}} {{command}}`

- Run a command with options in a specific chroot:

`schroot --chroot {{chroot}} {{command}} -- {{command_options}}`

- Run a command in all available chroots:

`schroot --all {{command}}`

- Start an interactive shell within a specific chroot as a specific user:

`schroot --chroot {{chroot}} --user {{user}}`

- List available chroots:

`schroot --list`
