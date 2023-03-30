# docker ps 
## chatgpt 
The `docker ps` command is used to display the list of all the currently running Docker containers on a Docker host. 
It outputs a table with the following columns: 

1. CONTAINER ID: A unique identifier for the container. 
2. IMAGE: The name and tag of the Docker image used to create the container. 
3. COMMAND: The command that was executed when the container was started. 
4. CREATED: The time and date the container was created. 
5. STATUS: The current status of the container (e.g., running, stopped, paused, restarting). 
6. PORTS: The ports to which the container is bound (e.g., 80/tcp). 
7. NAMES: The name of the container. 

The `docker ps` command without any arguments will only show the currently running containers. If the user wants to see all the containers (including those that are not running), they can use the `-a` or `--all` option.

Overall, the `docker ps` command is essential for managing and monitoring the Docker containers in a system. 

## tldr 
 
> List Docker containers.
> More information: <https://docs.docker.com/engine/reference/commandline/ps/>.

- List currently running docker containers:

`docker ps`

- List all docker containers (running and stopped):

`docker ps --all`

- Show the latest created container (includes all states):

`docker ps --latest`

- Filter containers that contain a substring in their name:

`docker ps --filter="name={{name}}"`

- Filter containers that share a given image as an ancestor:

`docker ps --filter "ancestor={{image}}:{{tag}}"`

- Filter containers by exit status code:

`docker ps --all --filter="exited={{code}}"`

- Filter containers by status (created, running, removing, paused, exited and dead):

`docker ps --filter="status={{status}}"`

- Filter containers that mount a specific volume or have a volume mounted in a specific path:

`docker ps --filter="volume={{path/to/directory}}" --format "table {{.ID}}\t{{.Image}}\t{{.Names}}\t{{.Mounts}}"`
