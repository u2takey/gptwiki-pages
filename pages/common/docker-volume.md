# docker volume 
## chatgpt 
The `docker volume` command in Docker is used to manage volumes, which are a way to persist data and share it among containers. Volumes are a key concept in Docker and are used to store data that needs to persist beyond the life of a container, as the data is not lost when the container is removed. 

The `docker volume` command allows you to create, list, inspect, remove, and prune volumes. 

Some common subcommands for `docker volume` are:

- `create`: This subcommand is used to create a new volume.
- `ls` or `list`: This subcommand is used to list all the volumes.
- `inspect`: This subcommand is used to inspect the details of a specific volume.
- `rm` or `remove`: This subcommand is used to remove a specific volume.
- `prune`: This subcommand is used to remove all unused volumes. 

For example, to create a new volume named `my-volume`, you can run the command:

```
docker volume create my-volume
```

To list all the existing volumes, you can run:

```
docker volume list
```

To inspect the details of a specific volume (e.g., `my-volume`), you can run:

```
docker volume inspect my-volume
```

To remove a specific volume (e.g., `my-volume`), you can run:

```
docker volume rm my-volume
```

To remove all unused volumes, you can run:

```
docker volume prune
```

Overall, the `docker volume` command is essential for working with Docker volumes and managing persistent data in containers. 

## tldr 
 
> Manage Docker volumes.
> More information: <https://docs.docker.com/engine/reference/commandline/volume/>.

- Create a volume:

`docker volume create {{volume_name}}`

- Create a volume with a specific label:

`docker volume create --label {{label}} {{volume_name}}`

- Create a `tmpfs` volume a size of 100 MiB and an uid of 1000:

`docker volume create --opt {{type}}={{tmpfs}} --opt {{device}}={{tmpfs}} --opt {{o}}={{size=100m,uid=1000}} {{volume_name}}`

- List all volumes:

`docker volume ls`

- Remove a volume:

`docker volume rm {{volume_name}}`

- Display information about a volume:

`docker volume inspect {{volume_name}}`

- Remove all unused local volumes:

`docker volume prune`

- Display help for a subcommand:

`docker volume {{subcommand}} --help`
