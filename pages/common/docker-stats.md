# docker stats 
## chatgpt 
The `docker stats` command is used to display live performance statistics for all running containers on a Docker host. When this command is executed, Docker pulls the latest statistics for all containers that are currently running and displays the following information:

- CONTAINER ID: A unique identifier for each running container
- NAME: The name assigned to the container
- CPU %: The percentage of CPU usage for each container
- MEM USAGE/LIMIT: The amount of memory used and the total memory limit for each container
- MEM %: The percentage of memory used by each container
- NET I/O: The input and output data rate for each container's network
- BLOCK I/O: The input/output data rate for each container's block device
- PIDS: The total number of processes running in each container

This command is useful for monitoring the performance of running containers and identifying potential performance issues. It can also help in making decisions regarding scaling of containers or resource allocation. 

## tldr 
 
> Display a live stream of resource usage statistics for containers.
> More information: <https://docs.docker.com/engine/reference/commandline/stats/>.

- Display a live stream for the statistics of all running containers:

`docker stats`

- Display a live stream of statistics for a space-separated list of containers:

`docker stats {{container_name}}`

- Change the columns format to display container's CPU usage percentage:

`docker stats --format "{{.Name}}:\t{{.CPUPerc}}"`

- Display statistics for all containers (both running and stopped):

`docker stats --all`

- Disable streaming stats and only pull the current stats:

`docker stats --no-stream`
