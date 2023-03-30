# podman image 
## chatgpt 
The "podman image" command is a subcommand used in the Podman container engine. It is used to manage images, which are the basis for creating container instances.

Here are the most commonly used subcommands with "podman image":

1. "podman image list": This command lists all the images available locally.

2. "podman image pull": This command downloads an image from a registry.

3. "podman image push": This command uploads an image to a registry.

4. "podman image build": This command builds an image from a Dockerfile or a Podmanfile.

5. "podman image inspect": This command displays detailed information about an image, including the layers it contains and its configuration.

6. "podman image rm": This command removes one or more images from the local image store.

7. "podman image save": This command saves one or more images to a tar archive.

8. "podman image load": This command loads one or more images from a tar archive.

In summary, the "podman image" command is an essential tool for managing images in the Podman container engine, allowing developers to retrieve, create, delete, and upload images to a registry. 

## tldr 
 
> Manage Docker images.
> See also `podman build`, `podman import`, and `podman pull`.
> More information: <https://docs.podman.io/en/latest/markdown/podman-image.1.html>.

- List local Docker images:

`podman image ls`

- Delete unused local Docker images:

`podman image prune`

- Delete all unused images (not just those without a tag):

`podman image prune --all`

- Show the history of a local Docker image:

`podman image history {{image}}`
