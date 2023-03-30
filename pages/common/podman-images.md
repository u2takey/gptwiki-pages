# podman images 
## chatgpt 
The "podman images" command is used in a Linux or Unix based operating system to list all the container images present on the local system, including their image name, tag, and size.

When you execute the "podman images" command, the following information is displayed:

1. Repository: This column displays the name of the image.
2. Tag: This column displays the tag of the image.
3. Image ID: This column displays the unique ID of the image.
4. Created: This column displays the date and time when the image was created.
5. Size: This column displays the size of the image.

The "podman images" command helps users to keep track of all the images that are stored on their machine. This is useful when you want to see the list of images before running them, or to remove unused or unwanted images to free up disk space. 

## tldr 
 
> Manage Podman images.
> More information: <https://docs.podman.io/en/latest/markdown/podman-images.1.html>.

- List all Podman images:

`podman images`

- List all Podman images including intermediates:

`podman images --all`

- List the output in quiet mode (only numeric IDs):

`podman images --quiet`

- List all Podman images not used by any container:

`podman images --filter dangling=true`

- List images that contain a substring in their name:

`podman images "{{*image|image*}}"`
