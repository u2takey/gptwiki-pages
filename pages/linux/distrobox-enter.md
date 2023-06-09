# distrobox-enter 
## chatgpt 
As an AI language model, I do not have access to the context or specific tool or software that you are referring to. However, based on my general knowledge, "distrobox-enter" could be a command line or terminal command used to enter a Linux distribution box or environment, similar to "chroot" but designed for distributing software in isolated containers. It may be used to manage or access different distributions, applications or services within a single host or system, without affecting its base or main operating system. Without more information about the tool or software where the "distrobox-enter" command is used, it is difficult to provide more specific detail or explanation. 

## tldr 
 
> Enter a distrobox container. See also: `tldr distrobox`.
> Default command executed is your SHELL, but you can specify different shells or entire commands to execute. If used inside a script, an application, or a service, you can use the `--headless` mode to disable the tty and interactivity.
> More information: <https://distrobox.privatedns.org/usage/distrobox-enter.html>.

- Enter a distrobox container:

`distrobox-enter {{container_name}}`

- Enter a distrobox container and run a command at login:

`distrobox-enter {{container_name}} -- {{sh -l}}`

- Enter a distrobox container without instantiating a tty:

`distrobox-enter --name {{container_name}} -- {{uptime -p}}`
