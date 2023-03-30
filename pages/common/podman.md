# podman 
## chatgpt 
Podman is a command-line utility tool that is used for managing containers on Linux systems. It is an alternative to Docker, and it is designed to be more secure and lightweight.

Here are some of the most common commands used with Podman:

1. podman run - This command is used to create a new container and start it. It takes the container image name and any additional parameters needed to launch the container as arguments.

2. podman ps - This command is used to list all the running containers on the system.

3. podman images - This command is used to list all the container images available on the system.

4. podman build - This command is used to build a new container image from a Dockerfile or a YAML file.

5. podman stop - This command is used to stop a running container.

6. podman rm - This command is used to remove a stopped container.

7. podman logs - This command is used to view the logs of a container.

8. podman exec - This command is used to execute a command in a running container.

These are just some of the most common commands used with Podman. There are many more commands available, and each of them has several options and arguments to customize their behavior. 

## tldr 
 
> Simple management tool for pods, containers and images.
> Podman provides a Docker-CLI comparable command-line. Simply put: `alias docker=podman`.
> More information: <https://github.com/containers/podman/blob/main/commands-demo.md>.

- List all containers (both running and stopped):

`podman ps --all`

- Create a container from an image, with a custom name:

`podman run --name {{container_name}} {{image}}`

- Start or stop an existing container:

`podman {{start|stop}} {{container_name}}`

- Pull an image from a registry (defaults to Docker Hub):

`podman pull {{image}}`

- Display the list of already downloaded images:

`podman images`

- Open a shell inside an already running container:

`podman exec --interactive --tty {{container_name}} {{sh}}`

- Remove a stopped container:

`podman rm {{container_name}}`

- Display the logs of one or more containers and follow log output:

`podman logs --follow {{container_name}} {{container_id}}`
