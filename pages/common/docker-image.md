# docker image 
## chatgpt 
"Docker image" is not a command in Docker, it is a term used to refer to the building blocks of Docker containers. 

Docker images are essentially templates or blueprints that define how a container will run. They contain all the necessary components, such as the operating system, application code, and dependencies. When a Docker container is started from an image, a new instance of the image is created, and any changes made to the container are isolated from the original image.

To see a list of the Docker images that are available on your system, you can use the "docker images" command. This command will show you the name of the image, its ID, the version or tag, the image size, and when the image was created.

For example, running the command "docker images" might show output similar to the following:

```
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
ubuntu              latest              2ca708c1c9cc        5 days ago          73.9MB
nginx               latest              41e8931bea87        5 days ago          133MB
postgres            latest              bdeaa09eb730        5 days ago          374MB
```

This output shows that there are three Docker images available on the system: Ubuntu, Nginx, and PostgreSQL, each with a different tag (or version). The IMAGE ID is a unique identifier for each image. The CREATED column shows how long ago the image was built, and the SIZE column shows the size of each image. 

## tldr 
 
> Manage Docker images.
> See also `docker build`, `docker import`, and `docker pull`.
> More information: <https://docs.docker.com/engine/reference/commandline/image/>.

- List local Docker images:

`docker image ls`

- Delete unused local Docker images:

`docker image prune`

- Delete all unused images (not just those without a tag):

`docker image prune --all`

- Show the history of a local Docker image:

`docker image history {{image}}`
