# docker compose 
## chatgpt 
The docker-compose command is used to create and manage multi-container Docker applications. It allows you to define your application’s services, networks, and volumes in a YAML file, and then spin up everything with a single command. 

Here's how it works:

1. Create a docker-compose.yml file that describes your application’s infrastructure. This file specifies which Docker images to use for each service, how to configure each service, and how to connect them together.

2. Use the docker-compose command to start, stop, or restart your application. You can also use it to scale your application up or down, by adding or removing containers.

3. Docker Compose ensures that your containers are started in the correct order, and that they have access to the resources they need, such as network connections and volumes.

4. Docker Compose also allows you to define different environments for your application, such as production, development, or testing. You can switch between these environments by specifying a different Compose file or environmental variables.

5. With Docker Compose, you can easily manage complex applications that require multiple containers, such as web servers, databases, messaging systems, and more. 

Overall, Docker Compose simplifies the deployment and management of multi-container Docker applications, making it easier to get your application up and running, while also improving scalability and flexibility. 

## tldr 
 
> Run and manage multi container docker applications.
> More information: <https://docs.docker.com/compose/reference/>.

- List all running containers:

`docker compose ps`

- Create and start all containers in the background using a `docker-compose.yml` file from the current directory:

`docker compose up --detach`

- Start all containers, rebuild if necessary:

`docker compose up --build`

- Start all containers using an alternate compose file:

`docker compose --file {{path/to/file}} up`

- Stop all running containers:

`docker compose stop`

- Stop and remove all containers, networks, images, and volumes:

`docker compose down --rmi all --volumes`

- Follow logs for all containers:

`docker compose logs --follow`

- Follow logs for a specific container:

`docker compose logs --follow {{container_name}}`
