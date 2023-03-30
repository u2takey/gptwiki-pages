# podman build 
## chatgpt 
The "podman build" command is used to build a new container image from the Dockerfile of the application. It is a part of the Podman container management tool, which is an alternative to the Docker container management system and runs without root privileges.

The basic syntax of the "podman build" command is as follows:

podman build [OPTIONS] PATH

Where "OPTIONS" can include various additional parameters to modify the build process such as:

- "-t" or "--tag": allows you to set the name and optionally a tag of the new image.
- "-f" or "--file": specifies the location of the Dockerfile to use for the build.
- "-q" or "--quiet": disables the build output, and only displays the final image ID.
- "-m" or "--memory": limits the amount of memory used for the build process.
- "-c" or "--cpu-shares": sets the CPU shares (relative weight) for the build process.
- "--no-cache": disables the use of the build cache, forcing a new build from scratch.
- "--security-opt": sets various security options for the container, such as SELinux or AppArmor.

The "PATH" parameter specifies the path to the build context, which is the directory containing the Dockerfile and any additional files needed for the build.

During the build process, Podman will execute the commands and instructions listed in the Dockerfile and create a new container image based on them. The resulting image can be saved or pushed to a registry for later use.

Overall, the "podman build" command is a powerful tool to create customized container images with specific configurations, dependencies, and applications. 

## tldr 
 
> Daemonless tool for building container images.
> Podman provides a Docker-CLI comparable command-line. Simply put: `alias docker=podman`.
> More information: <https://docs.podman.io/en/latest/markdown/podman-build.1.html>.

- Create an image using a `Dockerfile` or `Containerfile` in the specified directory:

`podman build {{path/to/directory}}`

- Create an image with a specified tag:

`podman build --tag {{image_name:version}} {{path/to/directory}}`

- Create an image from a non-standard file:

`podman build --file {{Containerfile.different}} .`

- Create an image without using any previously cached images:

`podman build --no-cache {{path/to/directory}}`

- Create an image suppressing all output:

`podman build --quiet {{path/to/directory}}`
