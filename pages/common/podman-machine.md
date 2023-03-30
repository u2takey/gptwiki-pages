# podman machine 
## chatgpt 
The "podman machine" command is not a recognized command in Podman. There is no official command named "podman machine" in any version of Podman.

However, there is a third-party tool called "podman-machine" that provides a way to provision and manage virtual machines for running Podman containers.

The "podman-machine" command is used to create, manage, and connect to virtual machines. It is similar to the Docker Machine tool used for managing Docker hosts.

The "podman-machine" tool creates virtual machines using various virtualization technologies such as VirtualBox, Hyper-V, or KVM. Once the virtual machine is created, Podman can be used to run containers within the virtual machine.

To use "podman-machine", you need to first install it on your system. Once installed, you can run "podman-machine create" to create a new virtual machine, and "podman-machine start" to start it. You can then use "podman-machine env" to set up the environment variables needed to connect to the virtual machine.

Overall, "podman-machine" makes it easy to create and manage virtual machines for running Podman containers. 

## tldr 
 
> Create and manage virtual machines running Podman.
> Included with Podman version 4 or greater.
> More information: <https://docs.podman.io/en/latest/markdown/podman-machine.1.html>.

- List existing machines:

`podman machine ls`

- Create a new default machine:

`podman machine init`

- Create a new machine with a specific name:

`podman machine init {{name}}`

- Create a new machine with different resources:

`podman machine init --cpus={{4}} --memory={{4096}} --disk-size={{50}}`

- Start or stop a machine:

`podman machine {{start|stop}} {{name}}`

- Connect to a running machine via SSH:

`podman machine ssh {{name}}`

- Inspect information about a machine:

`podman machine inspect {{name}}`
