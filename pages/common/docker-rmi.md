# docker rmi 
## chatgpt 
The docker rmi command is used to remove one or more Docker images from the local host system. The syntax of the command is:

```docker rmi [OPTIONS] IMAGE [IMAGE...]```

Where IMAGE is the name or ID of the Docker image to be removed, and OPTIONS can be used to specify additional settings.

Some of the frequently used options with the docker rmi command are:

- -f or --force: This option forces the removal of the docker images, even if they are being used by containers. It is a good practice to stop all running containers using the image before running this option.
- -no-prune: This option tells docker not to remove the parent images when they become orphaned. Orphaned images are the ones whose child images have been removed, and they are no longer used by any container.
- --filter: This option is used to filter the images to be removed based on their label, name, or ID. Multiple filters can be used simultaneously.

Note that, by default, docker images are cached on the local host, and docker rmi only removes images when they are not in use by any running or stopped containers. Therefore, before running the rmi command, it is recommended to stop and remove all the containers that are using the image or images to be deleted. 

## tldr 
 
> Remove one or more Docker images.
> More information: <https://docs.docker.com/engine/reference/commandline/rmi/>.

- Show help:

`docker rmi`

- Remove one or more images given their names:

`docker rmi {{image1 image2 ...}}`

- Force remove an image:

`docker rmi --force {{image}}`

- Remove an image without deleting untagged parents:

`docker rmi --no-prune {{image}}`
