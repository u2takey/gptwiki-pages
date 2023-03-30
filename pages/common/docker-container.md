# docker container 
## chatgpt 
"docker container" is a command used in the Docker platform to manage Docker containers. Docker containers are lightweight and standalone executable packages that contain everything needed to run an application or a service, including the code, runtime, system tools, libraries, and settings.

The "docker container" command is used to create, start, stop, restart, remove, and manage Docker containers. Some of the commonly used sub-commands with "docker container" include:

- docker container create: This command is used to create a new Docker container from scratch.

- docker container start: This command is used to start a stopped Docker container.

- docker container stop: This command is used to stop a running Docker container.

- docker container restart: This command is used to restart a running Docker container.

- docker container rm: This command is used to remove one or more Docker containers.

Additionally, the "docker container" command can also be used to view information about running containers, inspect container configurations, logs, and network settings.

In summary, "docker container" is a powerful command used to manage and work with Docker containers from the command line interface. 

## tldr 
 
> Manage Docker containers.
> More information: <https://docs.docker.com/engine/reference/commandline/container/>.

- List currently running Docker containers:

`docker container ls`

- Start one or more stopped containers:

`docker container start {{container1_name}} {{container2_name}}`

- Kill one or more running containers:

`docker container kill {{container_name}}`

- Stop one or more running containers:

`docker container stop {{container_name}}`

- Pause all processes within one or more containers:

`docker container pause {{container_name}}`

- Display detailed information on one or more containers:

`docker container inspect {{container_name}}`

- Export a container's filesystem as a tar archive:

`docker container export {{container_name}}`

- Create a new image from a container's changes:

`docker container commit {{container_name}}`
