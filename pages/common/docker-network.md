# docker network 
## chatgpt 
Docker network is a command in Docker that is used to manage Docker networks. Docker networking provides a way for containers to communicate with each other and with the outside world. With Docker networking, you can create virtual networks, attach containers to them, and even connect containers on different hosts.

To use the docker network command, you must have Docker installed on your system. Once Docker is installed, you can use the docker network command to create, inspect, and manage Docker networks. Here is an overview of the different functions that you can perform with the docker network command:

1. create: This command is used to create a new Docker network. You can specify the driver that the network will use and any other options that you want to set.

2. connect: This command is used to connect a container to a Docker network. You can specify the container ID or name and the network name.

3. disconnect: This command is used to disconnect a container from a Docker network. You can specify the container ID or name and the network name.

4. ls: This command is used to list all the Docker networks on your system.

5. inspect: This command is used to inspect a specific Docker network. You can specify the network ID or name.

6. rm: This command is used to remove a Docker network. You can specify the network ID or name.

Overall, the docker network command is a powerful tool for managing Docker networks and making sure that your containers are able to communicate with each other and the outside world. 

## tldr 
 
> Create and manage docker networks.
> More information: <https://docs.docker.com/engine/reference/commandline/network/>.

- List all available and configured networks on docker daemon:

`docker network ls`

- Create a user-defined network:

`docker network create --driver {{driver_name}} {{network_name}}`

- Display detailed information of a space-separated list of networks:

`docker network inspect {{network_name}}`

- Connect a container to a network using a name or ID:

`docker network connect {{network_name}} {{container_name|ID}}`

- Disconnect a container from a network:

`docker network disconnect {{network_name}} {{container_name|ID}}`

- Remove all unused (not referenced by any container) networks:

`docker network prune`

- Remove a space-separated list of unused networks:

`docker network rm {{network_name}}`
