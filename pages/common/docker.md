# docker 
## chatgpt 
I'm sorry, but the command "docker" is not specific enough for me to provide a detailed explanation. Docker is a command-line interface that provides a way to build, run and manage Docker containers. To use the Docker command, you need to specify a sub-command after "docker". Some examples of sub-commands are:

- docker run: Let you run a Docker container from an image.
- docker build: Let you create a Docker image from a Dockerfile.
- docker images: List all the Docker images on your system.
- docker ps: List all the running Docker containers.

Every sub-command has its own parameters and options that you can use to customize its behavior. You can get more information about each sub-command by typing "docker <sub-command> --help". 

## tldr 
 
> Manage Docker containers and images.
> Some subcommands such as `docker run` have their own usage documentation.
> More information: <https://docs.docker.com/engine/reference/commandline/cli/>.

- List all docker containers (running and stopped):

`docker ps --all`

- Start a container from an image, with a custom name:

`docker run --name {{container_name}} {{image}}`

- Start or stop an existing container:

`docker {{start|stop}} {{container_name}}`

- Pull an image from a docker registry:

`docker pull {{image}}`

- Display the list of already downloaded images:

`docker images`

- Open a shell inside a running container:

`docker exec -it {{container_name}} {{sh}}`

- Remove a stopped container:

`docker rm {{container_name}}`

- Fetch and follow the logs of a container:

`docker logs -f {{container_name}}`
