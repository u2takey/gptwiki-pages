# needrestart 
## chatgpt 
The "needrestart" command is used on Unix-like systems to identify processes that need to be restarted after a system upgrade, such as a kernel or libraries upgrade. When you upgrade the system, some applications or services may be using older versions of libraries, which may cause stability or security issues. The "needrestart" command will identify such processes and display a list of actions needed to restart them, such as restarting the service or rebooting the system.

The "needrestart" command is generally used in two ways:

1. Checking for needrestart: By default, the command will check for processes that need to be restarted after a system upgrade. You can run the command without any options to see the list of services, daemons, or applications that need to be restarted.

2. Reloading/restarting affected services: If you want to reload or restart the services, daemons, or applications that need to be restarted after an upgrade, you can use the command with specific options. The options are:

- "-r" or "--restart": This option will restart or reload the affected services.

- "-p" or "--postponed": This option will only display a list of processes that need to be restarted, but will not restart or reload them.

- "-h" or "--help": This option will display the help page with a brief description of other available options.

Overall, the "needrestart" command is a helpful tool in maintaining a stable and secure system after a system upgrade, as it can identify and restart processes that may cause issues with the new system version. 

## tldr 
 
> Check which daemons need to be restarted after library upgrades.
> More information: <https://github.com/liske/needrestart>.

- List outdated processes:

`needrestart`

- Interactively restart services:

`sudo needrestart`

- List outdated processes in [v]erbose or [q]uiet mode:

`needrestart -{{v|q}}`

- Check if the [k]ernel is outdated:

`needrestart -k`

- Check if the CPU microcode is outdated:

`needrestart -w`

- List outdated processes in [b]atch mode:

`needrestart -b`

- List outdated processed using a specific [c]onfiguration file:

`needrestart -c {{path/to/config}}`

- Display help:

`needrestart --help`
