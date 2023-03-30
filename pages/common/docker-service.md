# docker service 
## chatgpt 
The `docker service` command is used to manage services in a Docker Swarm cluster. A service in Docker is a definition of a desired state for running containers, including the number of replicas, networking details, and more. 

The `docker service` command can be used to perform various operations on a service, such as creating, updating, scaling, inspecting, or deleting it. 

Here are some common examples of using the `docker service` command:

- `docker service create`: This command is used to create a new service with the specified properties, such as the image to use, the number of replicas, the network configuration, and more. For example: `docker service create --name my-web-app --replicas 3 --publish 80:80 nginx:latest` creates a new service called `my-web-app` with three replicas running the `nginx` image, and exposes port 80 to the world.

- `docker service update`: This command is used to update an existing service with new properties, such as the number of replicas, the image to use, and more. For example: `docker service update --replicas 5 my-web-app` updates the `my-web-app` service to have five replicas instead of its current number.

- `docker service scale`: This command is used to scale a service up or down, by adding or removing replicas. For example: `docker service scale my-web-app=7` increases the number of replicas of the `my-web-app` service to seven.

- `docker service ls`: This command is used to list all the services running in the Swarm cluster, and their status, replicas, and other properties. 

- `docker service logs`: This command is used to view the logs of a service, by concatenating the logs of all its replicas. 

Overall, the `docker service` command is an essential tool for managing services in a Docker Swarm cluster, and allows you to automate and scale your applications with ease. 

## tldr 
 
> Manage the services on a docker daemon.
> More information: <https://docs.docker.com/engine/reference/commandline/service/>.

- List the services on a docker daemon:

`docker service ls`

- Create a new service:

`docker service create --name {{service_name}} {{image}}:{{tag}}`

- Display detailed information of a space-separated list of services:

`docker service inspect {{service_name|ID}}`

- List the tasks of a space-separated list of services:

`docker service ps {{service_name|ID}}`

- Scale to a specific number of replicas for a space-separated list of services:

`docker service scale {{service_name}}={{count_of_replicas}}`

- Remove a space-separated list of services:

`docker service rm {{service_name|ID}}`
