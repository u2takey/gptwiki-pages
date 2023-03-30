# podman ps 
## chatgpt 
The `podman ps` command is used to list all the currently running containers within the Podman environment. It displays information about the containers such as their names, status, unique IDs (or container IDs), the images they are based on, and the port mappings they use.

Here is a breakdown of each component of the command:

- `podman` is the command-line tool for managing containers and images.
- `ps` is a sub-command that stands for "process status" and is commonly used to list running processes.

When executed, the `podman ps` command generates a table with each container's information that is easy to read and interpret. This information can be helpful for troubleshooting, debugging, or managing your containers in general. 

## tldr 
 
> List Podman containers.
> More information: <https://docs.podman.io/en/latest/markdown/podman-ps.1.html>.

- List currently running podman containers:

`podman ps`

- List all podman containers (running and stopped):

`podman ps --all`

- Show the latest created container (includes all states):

`podman ps --latest`

- Filter containers that contain a substring in their name:

`podman ps --filter="name={{name}}"`

- Filter containers that share a given image as an ancestor:

`podman ps --filter "ancestor={{image}}:{{tag}}"`

- Filter containers by exit status code:

`podman ps --all --filter="exited={{code}}"`

- Filter containers by status (created, running, removing, paused, exited and dead):

`podman ps --filter="status={{status}}"`

- Filter containers that mount a specific volume or have a volume mounted in a specific path:

`podman ps --filter="volume={{path/to/directory}}" --format "table {{.ID}}\t{{.Image}}\t{{.Names}}\t{{.Mounts}}"`
