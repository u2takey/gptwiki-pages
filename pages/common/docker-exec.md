# docker exec 
## chatgpt 
The `docker exec` command allows the user to run a command inside a running Docker container. 

The syntax for `docker exec` is as follows:

```
docker exec [OPTIONS] CONTAINER COMMAND [ARG...]
```

* `OPTIONS`: Additional options to configure the behavior of the command. Some common options include `-i` (keep STDIN open even if not attached), `-t`(allocate a pseudo-TTY), and `--user` (run the command as a specified user).
* `CONTAINER`: The name or ID of the Docker container to execute the command inside.
* `COMMAND`: The command to be executed inside the container.
* `ARG`: Optional arguments passed to the command.

For example, the following command will execute the `ls` command inside a container named `my_container`:

```
docker exec my_container ls
```

This will list the contents of the current directory inside the `my_container`. 

Note that `docker exec` only works on running containers, and the container must be started with `-d` or `--detach` flag to be able to use it. 

## tldr 
 
> Execute a command on an already running Docker container.
> More information: <https://docs.docker.com/engine/reference/commandline/exec/>.

- Enter an interactive shell session on an already-running container:

`docker exec --interactive --tty {{container_name}} {{/bin/bash}}`

- Run a command in the background (detached) on a running container:

`docker exec --detach {{container_name}} {{command}}`

- Select the working directory for a given command to execute into:

`docker exec --interactive -tty --workdir {{path/to/directory}} {{container_name}} {{command}}`

- Run a command in background on existing container but keep `stdin` open:

`docker exec --interactive --detach {{container_name}} {{command}}`

- Set an environment variable in a running Bash session:

`docker exec --interactive --tty --env {{variable_name}}={{value}} {{container_name}} {{/bin/bash}}`

- Run a command as a specific user:

`docker exec --user {{user}} {{container_name}} {{command}}`
