# lxc 
## chatgpt 
The command "lxc" is used to manage LXC (Linux Containers). LXC is an operating system-level virtualization technology that allows multiple isolated Linux systems (containers) to run on a single Linux host. 

The "lxc" command can be used for various purposes such as creating, starting, stopping, deleting, cloning, and managing containers. Some of the commonly used sub-commands of "lxc" are:

1. lxc-create: This is used to create a new container. It requires specifying the name of the container and the template to use for creating it.

2. lxc-start: This is used to start a container.

3. lxc-stop: This is used to stop a container.

4. lxc-destroy: This is used to destroy a container.

5. lxc-info: This is used to display information about a container such as the state, PID, IP address, etc.

6. lxc-attach: This is used to attach to a running container and run commands inside it.

7. lxc-ls: This is used to list all the containers that are currently created.

Overall, the "lxc" command is a powerful tool for managing Linux containers and offers a wide range of options for creating, managing, and monitoring them. 

## tldr 
 
> Manage Linux containers using the lxd REST API.
> Any container names or patterns can be prefixed with the name of a remote server.
> More information: <https://manned.org/lxc>.

- List local containers matching a string. Omit the string to list all local containers:

`lxc list {{match_string}}`

- List images matching a string. Omit the string to list all images:

`lxc image list [{{remote}}:]{{match_string}}`

- Create a new container from an image:

`lxc init [{{remote}}:]{{image}} {{container}}`

- Start a container:

`lxc start [{{remote}}:]{{container}}`

- Stop a container:

`lxc stop [{{remote}}:]{{container}}`

- Show detailed info about a container:

`lxc info [{{remote}}:]{{container}}`

- Take a snapshot of a container:

`lxc snapshot [{{remote}}:]{{container}} {{snapshot}}`

- Execute a specific command inside a container:

`lxc exec [{{remote}}:]{{container}} {{command}}`
