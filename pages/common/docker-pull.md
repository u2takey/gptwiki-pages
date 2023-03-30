# docker pull 
## chatgpt 
The `docker pull` command is used to download a Docker image from a container registry. When you run this command, Docker will search for the specified image in the registry, and if it is available, it will download the image onto your local system. The `pull` command fetches an image from the Docker Hub or from a container registry specified with a URL.

Syntax:

```
docker pull [OPTIONS] NAME[:TAG|@DIGEST]
```

- `OPTIONS`: Optional parameters that modify the behavior of the `pull` command.
- `NAME`: The name of the Docker image to download.
- `TAG`: The tag of the Docker image to download. If not specified, Docker will download the default `latest` tag if available.
- `DIGEST`: The unique identifier of the specific image version, which Docker uses to identify a specific image.

Once a Docker image is downloaded onto your system, it can be used to create Docker containers. This `docker pull` is one of the fundamental and frequent used commands when working with Docker-based projects. 

## tldr 
 
> Download Docker images from a registry.
> More information: <https://docs.docker.com/engine/reference/commandline/pull/>.

- Download a specific Docker image:

`docker pull {{image}}:{{tag}}`

- Download a specific Docker image in quiet mode:

`docker pull --quiet {{image}}:{{tag}}`

- Download all tags of a specific Docker image:

`docker pull --all-tags {{image}}`

- Download a Docker images for a specific platform, e.g. linux/amd64:

`docker pull --platform {{linux/amd64}} {{image}}:{{tag}}`

- Display help:

`docker pull --help`
