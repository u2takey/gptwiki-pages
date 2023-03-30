# docker start 
## chatgpt 
The `docker start` command is used to start one or more stopped Docker containers. The syntax for the command is as follows:

```
docker start [OPTIONS] CONTAINER [CONTAINER...]
```

- `OPTIONS`: Optional parameters that can be added to the command to modify its behavior.
- `CONTAINER`: The name or ID of the container(s) that needs to be started.

When a Docker container is stopped, it is not running and its resources are not being used. The `docker start` command starts the container again and provides access to its resources, including its file system and network settings. The container will resume the same state it was in when it was stopped, with all its running processes, open files, and network connections unchanged.

Some of the commonly used options with `docker start` command are:

- `-a` or `--attach`: Attach STDOUT/STDERR and display the output on the console.
- `-i` or `--interactive`: Keep STDIN open even if not attached.
- `-d` or `--detach`: Run container in the background and print container ID.

For example, to start a stopped container with ID `e7ad352341e5`, the following command can be used:

```
docker start e7ad352341e5
```

If successful, the command will return the container ID. To confirm that the container is now running, the `docker ps` command can be executed. This will provide a list of all running containers. 

## tldr 
 
> Start one or more stopped containers.
> More information: <https://docs.docker.com/engine/reference/commandline/start/>.

- Show help:

`docker start`

- Start a docker container:

`docker start {{container}}`

- Start a container, attaching `stdout` and `stderr` and forwarding signals:

`docker start --attach {{container}}`

- Start one or more space-separated containers:

`docker start {{container(s)}}`
