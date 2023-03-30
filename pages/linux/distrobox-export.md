# distrobox-export 
## chatgpt 
As an AI language model, I don't have enough context to accurately describe the "distrobox-export" command. However, I can provide a general explanation about how command works in Linux.

In Linux, a command is simply an executable program that you can run in a terminal or as part of a script. In general, commands are used to perform specific functions or tasks on a Linux system.

Without context, it's difficult to say what the "distrobox-export" command does exactly. Still, based on its name, it might be a command used to export or backup a Linux distribution. The command might export specific configuration files, settings or the entire OS. The specific usage of the command and the scope of the export would depend on the implementation of the command. 

Overall, to use any command, you need to type its name in a terminal session along with any necessary options and arguments. Once executed, the command will execute and perform the desired task, in this case, exporting a Linux distribution. 

## tldr 
 
> Export app/service/binary from container to host OS.
> Subcommand of `distrobox`. See also: `tldr distrobox`.
> More information: <https://distrobox.privatedns.org/usage/distrobox-export.html>.

- Export an app from the container to the host (the desktop entry/icon will show up in your host system's application list):

`distrobox-export --app {{package_name}} --extra-flags "--foreground"`

- Export a binary from the container to the host:

`distrobox-export --bin {{path/to/binary}} --export-path {{path/to/binary_on_host}}`

- Export a binary from the container to the host (i.e.`$HOME/.local/bin`) :

`distrobox-export --bin {{path/to/binary}} --export-path {{path/to/export}}`

- Export a service from the container to the host (`--sudo` will run the service as root inside the container):

`distrobox-export --service {{package}} --extra-flags "--allow-newer-config" --sudo`

- Unexport/delete an exported application:

`distrobox-export --app {{package}} --delete`
