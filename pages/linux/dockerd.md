# dockerd 
## chatgpt 
The command `dockerd` is used to start the Docker daemon, which is responsible for managing and running Docker containers on a host system. When executed, the `dockerd` command initializes the Docker engine, which is responsible for executing and managing high-level Docker commands issued through the Docker CLI.

The `dockerd` command can be used with various options to specify different configurations for the Docker engine, such as specifying the location of the Docker socket file or the location of the Docker configuration file. Different options can be used to specify the desired configuration and behavior of the Docker engine.

When the `dockerd` command is executed, the Docker engine starts running on the host system and listens for commands from the Docker CLI. Users can then issue various high-level Docker commands to manage and interact with Docker containers.

Overall, the `dockerd` command is critical to the operation of Docker, as it starts the Docker engine and allows users to manage and run Docker containers on their host systems. 

## tldr 
 
> A persistent process to start and manage docker containers.
> More information: <https://docs.docker.com/engine/reference/commandline/dockerd/>.

- Run docker daemon:

`dockerd`

- Run docker daemon and config it to listen to specific sockets (UNIX and TCP):

`dockerd --host unix://{{path/to/tmp.sock}} --host tcp://{{ip}}`

- Run with specific daemon PID file:

`dockerd --pidfile {{path/to/pid_file}}`

- Run in debug mode:

`dockerd --debug`

- Run and set a specific log level:

`dockerd --log-level={{debug|info|warn|error|fatal}}`
