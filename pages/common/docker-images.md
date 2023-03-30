# docker images 
## chatgpt 
The `docker images` command is used to display a list of all the Docker images that are available on your system. This command will show you the repository, tag, image ID, creation time and size of each image available. 

The output of this command can be useful for understanding the contents of your Docker environment, as well as identifying any images that you may want to remove to free up disk space.

Here's a breakdown of the different parts of the output:

- REPOSITORY: This column shows the name of the repository where the image belongs to. For example, the repository could be from Docker Hub, a private registry or a locally-built image.

- TAG: This column shows the tag associated with the image. Tags are used to label different versions of an image.

- IMAGE ID: This column shows the unique ID of the image.

- CREATED: This column shows when the image was created.

- SIZE: This column shows the size of the image.

By default, the `docker images` command will display all images available on your local machine. You can specify a repository or image name to filter the output down to a specific image or set of images. 

## tldr 
 
> Manage Docker images.
> More information: <https://docs.docker.com/engine/reference/commandline/images/>.

- List all Docker images:

`docker images`

- List all Docker images including intermediates:

`docker images --all`

- List the output in quiet mode (only numeric IDs):

`docker images --quiet`

- List all Docker images not used by any container:

`docker images --filter dangling=true`

- List images that contain a substring in their name:

`docker images "{{*name*}}"`
