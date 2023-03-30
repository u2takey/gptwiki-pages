# docker inspect 
## chatgpt 
The `docker inspect` command is used to retrieve information about a Docker container or image. It provides in-depth details about a container or image, including its configuration, networks it is connected to, its current status, and more.

When you run the `docker inspect` command, you need to provide the name or ID of the container or image you want to inspect. The output of this command is a JSON object that contains all the detailed information about the container or image.

Here are some examples of the types of information you can retrieve with `docker inspect`:

- Network settings: You can use the command to see which networks the container is connected to, the IP address of the container, and other network-related settings.
- Container configuration: The command can show you the full configuration that was used when creating the container, including its entry point and command used to run the container.
- Volume information: You can use `docker inspect` to see which volumes a container is connected to and their locations on the host machine.
- Health checks: The command can display any health checks that have been configured for the container, along with their results.

Overall, `docker inspect` is a powerful tool that can provide detailed information about your containers and images, and help with troubleshooting issues that you may encounter while working with Docker. 

## tldr 
 
> Return low-level information on Docker objects.
> More information: <https://docs.docker.com/engine/reference/commandline/inspect/>.

- Show help:

`docker inspect`

- Display information about a container, image, or volume using a name or ID:

`docker inspect {{container|image|ID}}`

- Display a container's IP address:

`docker inspect --format='{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' {{container}}`

- Display the path to the container's log file:

`docker inspect --format='{{.LogPath}}' {{container}}`

- Display the image name of the container:

`docker inspect --format='{{.Config.Image}}' {{container}}`

- Display the configuration information as JSON:

`docker inspect --format='{{json .Config}}' {{container}}`

- Display all port bindings:

`docker inspect --format='{{range $p, $conf := .NetworkSettings.Ports}} {{$p}} -> {{(index $conf 0).HostPort}} {{end}}' {{container}}`
