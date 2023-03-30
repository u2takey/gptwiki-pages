# rc-update 
## chatgpt 
As an AI language model, I can explain the basic functionality and usage of the command "rc-update".

The "rc-update" command is a utility tool for managing the services that run on an openrc-based operating system. The tool is used to manage startup and shutdown services including the runlevel configuration for an OpenRC system. It is commonly used in Linux distributions like Gentoo, Alpine and Void Linux.

The "rc-update" command takes the following syntax/options:

rc-update [OPTIONS] ACTION [ARGS]

Where:
- OPTIONS: Additional arguments to modify the command's behavior.
- ACTION: The main purpose of the command, which is usually a verb that describes the action. Possible actions include "add", "delete", "show", etc.
- ARGS: Additional arguments that depend on the chosen action.

Here are some frequently used actions and their meanings.

1. add: Adds a new service or script to the current runlevel.
Syntax:
rc-update add [service_name] [runlevel]

Example:
rc-update add sshd default

2. delete: Removes a service or script from the current runlevel.
Syntax:
rc-update delete [service_name] [runlevel]

Example:
rc-update delete sshd

3. show: Displays the service configurations for the system.
Syntax:
rc-update show

Example:
rc-update show

Overall, the "rc-update" command is a useful tool for managing services in an OpenRC system, and can help users in configuring and managing their system services effectively. 

## tldr 
 
> Add and remove OpenRC services to and from runlevels.
> See also `openrc`.
> More information: <https://manned.org/rc-update>.

- List all services and the runlevels they are added to:

`rc-update show`

- Add a service to a runlevel:

`sudo rc-update add {{service_name}} {{runlevel}}`

- Delete a service from a runlevel:

`sudo rc-update delete {{service_name}} {{runlevel}}`

- Delete a service from all runlevels:

`sudo rc-update --all delete {{service_name}}`
