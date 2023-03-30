# docker-machine 
## chatgpt 
Docker-machine is a command-line tool used to create, manage, and connect to Docker hosts. It is used to configure Docker on a remote machine and acts as a wrapper around Docker commands to manage Docker machines as VirtualBox or other hosts.

Below are some important commands related to Docker-machine.

- `create`: This command creates one or more Docker machines with the given configuration parameters. For example, you can specify a driver (virtualbox, aws, azure, etc.), a name, and other settings to create a new Docker machine.

- `ls`: This command lists all Docker machines that are currently running or stopped.

- `start`: This command starts one or more Docker machines that are currently stopped.

- `stop`: This command stops one or more Docker machines that are currently running.

- `ssh`: This command allows you to ssh into a Docker machine to perform tasks or run Docker commands.

- `env`: This command displays the shell environment variables that you need to configure the Docker client to connect to a specific Docker machine.

Overall, Docker-machine is a helpful tool for managing Docker hosts and simplifying the process of creating and connecting to Docker machines. 

## tldr 
 
> Create and manage machines running Docker.
> More information: <https://docs.docker.com/machine/reference/>.

- List currently running docker machines:

`docker-machine ls`

- Create a new docker machine with specific name:

`docker-machine create {{name}}`

- Get the status of a machine:

`docker-machine status {{name}}`

- Start a machine:

`docker-machine start {{name}}`

- Stop a machine:

`docker-machine stop {{name}}`

- Inspect information about a machine:

`docker-machine inspect {{name}}`
