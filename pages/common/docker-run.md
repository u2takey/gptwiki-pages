# docker run 
## chatgpt 
The `docker run` command is used to create and start a new container based on a specified Docker image. This command is the most commonly used command for working with containers.

The basic syntax of the `docker run` command is:

```
docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
```

Here, `OPTIONS` are various configuration options that can be used to customize the container, including network settings, volume mapping, environment variables, etc. `IMAGE` is the name or ID of the Docker image that the container should be based on. `COMMAND` is an optional command to run inside the container, and `ARG` are any arguments to that command.

When you run this command, Docker starts by downloading the specified image (if it doesn't already exist on your system) and creating a new container based on that image. Docker then starts the container and runs any specified command inside it. 

If you don't specify a command, Docker runs the default command defined in the Docker image's metadata. When you execute this command, Docker assigns a randomly generated name to the container by default. 

Once the container is running, you can interact with it through the command line using the `docker exec` command, or you can access its application or service through the container's IP address and port number. 

Overall, the `docker run` command is a powerful tool for creating and managing Docker containers, allowing you to build, deploy, and run applications in a portable and scalable way. 

## tldr 
 
> Run a command in a new Docker container.
> More information: <https://docs.docker.com/engine/reference/commandline/run/>.

- Run command in a new container from a tagged image:

`docker run {{image:tag}} {{command}}`

- Run command in a new container in background and display its ID:

`docker run --detach {{image}} {{command}}`

- Run command in a one-off container in interactive mode and pseudo-TTY:

`docker run --rm --interactive --tty {{image}} {{command}}`

- Run command in a new container with passed environment variables:

`docker run --env '{{variable}}={{value}}' --env {{variable}} {{image}} {{command}}`

- Run command in a new container with bind mounted volumes:

`docker run --volume {{/path/to/host_path}}:{{/path/to/container_path}} {{image}} {{command}}`

- Run command in a new container with published ports:

`docker run --publish {{host_port}}:{{container_port}} {{image}} {{command}}`

- Run command in a new container overwriting the entrypoint of the image:

`docker run --entrypoint {{command}} {{image}}`

- Run command in a new container connecting it to a network:

`docker run --network {{network}} {{image}}`
