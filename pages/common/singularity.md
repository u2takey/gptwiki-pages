# singularity 
## chatgpt 
Singularity is a command-line tool used for creating, managing, and running container images. These images are lightweight, portable, and self-contained environments that can be used to run applications or perform tasks without interfering with the host system. 

Some of the common commands used in Singularity are:

1. `singularity build`: Used for creating a Singularity image from a recipe or a base image.
2. `singularity run`: Used for running a Singularity image as a container.
3. `singularity exec`: Used for running a specific command inside a Singularity container.
4. `singularity shell`: Used for opening an interactive shell inside a Singularity container.
5. `singularity pull`: Used for downloading and caching a Singularity image from a remote repository.

Singularity is often used in scientific computing and research, where reproducibility and portability of software environments are crucial. It can also be used for running Linux-based applications on systems without specific software requirements or dependencies. 

## tldr 
 
> Manage Singularity containers and images.
> More information: <https://singularity-docs.readthedocs.io/en/latest/#commands>.

- Download a remote image from Sylabs Cloud:

`singularity pull --name {{image.sif}} {{library://godlovedc/funny/lolcow:latest}}`

- Rebuild a remote image using the latest Singularity image format:

`singularity build {{image.sif}} {{docker://godlovedc/lolcow}}`

- Start a container from an image and get a shell inside it:

`singularity shell {{image.sif}}`

- Start a container from an image and run a command:

`singularity exec {{image.sif}} {{command}}`

- Start a container from an image and execute the internal runscript:

`singularity run {{image.sif}}`

- Build a singularity image from a recipe file:

`sudo singularity build {{image.sif}} {{recipe}}`
