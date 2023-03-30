# podman run 
## chatgpt 
The command "podman run" initiates a new container from an image. It is used to start and run a container using the specified image.

Here is the breakdown of the "podman run" command:

- "podman": This refers to the Podman container engine that allows you to manage containers.

- "run": This is a subcommand of Podman that is used to initiate and run a new container.

Here are some of the common options and arguments used with the "podman run" command:

- "-d" or "--detach": This option runs the container in detached mode, meaning it runs in the background without showing the container output.

- "-p" or "--publish": This option publishes container ports to the host. It maps the container's port to the host's port.

- "-e" or "--env": This option sets environment variables inside the container.

- "<image>": This is the argument that specifies the name of the image on which to base the container.

- "<command>": This is an optional argument that specifies the command to be run inside the container. If not specified, the default command defined in the image will run.

Overall, the "podman run" command is used to launch a new container from the specified image, with options and arguments used to customize the container's behavior during runtime. 

## tldr 
 
> Run a command in a new Podman container.
> More information: <https://docs.podman.io/en/latest/markdown/podman-run.1.html>.

- Run command in a new container from a tagged image:

`podman run {{image:tag}} {{command}}`

- Run command in a new container in background and display its ID:

`podman run --detach {{image:tag}} {{command}}`

- Run command in a one-off container in interactive mode and pseudo-TTY:

`podman run --rm --interactive --tty {{image:tag}} {{command}}`

- Run command in a new container with passed environment variables:

`podman run --env '{{variable}}={{value}}' --env {{variable}} {{image:tag}} {{command}}`

- Run command in a new container with bind mounted volumes:

`podman run --volume {{/path/to/host_path}}:{{/path/to/container_path}} {{image:tag}} {{command}}`

- Run command in a new container with published ports:

`podman run --publish {{host_port}}:{{container_port}} {{image:tag}} {{command}}`

- Run command in a new container overwriting the entrypoint of the image:

`podman run --entrypoint {{command}} {{image:tag}}`

- Run command in a new container connecting it to a network:

`podman run --network {{network}} {{image:tag}}`
