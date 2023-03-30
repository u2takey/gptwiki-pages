# docker system 
## chatgpt 
The command "docker system" is a subcommand of the Docker CLI (Command Line Interface) that provides management and troubleshooting functionality for the Docker system.

The "docker system" command has several subcommands that can be used to manage the Docker system. The available subcommands are:

1. "docker system df": This subcommand provides a summary of the Docker system's resource usage, including the amount of disk space used by Docker images, containers, and volumes.

2. "docker system events": This subcommand shows a real-time stream of Docker events, including container creation, deletion, and image pulls.

3. "docker system info": This subcommand displays information about the Docker system, such as the Docker version, the number of containers and images, and the status of the Docker daemon.

4. "docker system prune": This subcommand removes unused Docker resources, such as untagged images, stopped containers, and unused volumes.

5. "docker system trust": This subcommand manages the trust metadata for Docker content, including images and repository authentication.

In summary, "docker system" is a useful command for managing and maintaining the Docker system, providing insight into resource usage, event monitoring, system information, and resource cleanup. 

## tldr 
 
> Manage Docker data and display system-wide information.
> More information: <https://docs.docker.com/engine/reference/commandline/system/>.

- Show help:

`docker system`

- Show docker disk usage:

`docker system df`

- Show detailed information on disk usage:

`docker system df --verbose`

- Remove unused data:

`docker system prune`

- Remove unused data created more than a specified amount of time in the past:

`docker system prune --filter="until={{hours}}h{{minutes}}m"`

- Display real-time events from the Docker daemon:

`docker system events`

- Display real-time events from containers streamed as valid JSON Lines:

`docker system events --filter 'type=container' --format '{{json .}}'`

- Display system-wide information:

`docker system info`
