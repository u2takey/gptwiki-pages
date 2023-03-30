# podman-compose 
## chatgpt 
`podman-compose` is a command-line tool that provides a user-friendly way of managing containerized applications using Podman. It is a wrapper around the `podman` command and is used similarly to `docker-compose`. 

`podman-compose` is used to create and manage multi-container applications defined in a `docker-compose.yml` file. By running `podman-compose`, you can start, stop, and manage these applications with ease.

When you run `podman-compose`, it reads the `docker-compose.yml` file and creates one or more containers based on the services defined in the file. The services can include a web server, database, and other dependencies needed to run an application.

Some common `podman-compose` commands include:

- `up`: brings up the application and all its services
- `down`: stops and removes containers, networks, and volumes created by `up`
- `start`: starts containers that were previously created by `up`
- `stop`: stops running containers, but does not remove them
- `logs`: displays logs for the running containers

Overall, `podman-compose` makes it easier to manage multiple containers as a single application, streamlining the process of deployment and scaling. 

## tldr 
 
> Run and manage Compose Specification container definition.
> More information: <https://github.com/containers/podman-compose>.

- List all running containers:

`podman-compose ps`

- Create and start all containers in the background using a local `docker-compose.yml`:

`podman-compose up -d`

- Start all containers, building if needed:

`podman-compose up --build`

- Start all containers using an alternate compose file:

`podman-compose {{path/to/file}} up`

- Stop all running containers:

`podman-compose stop`

- Remove all containers, networks, and volumes:

`podman-compose down --volumes`

- Follow logs for a container (omit all container names):

`podman-compose logs --follow {{container_name}}`

- Run a one-time command in a service with no ports mapped:

`podman-compose run {{service_name}} {{command}}`
