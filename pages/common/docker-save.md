# docker save 
## chatgpt 
-Docker save command is used to save one or more Docker images to a TAR archive. This command allows you to archive your Docker image in a TAR format, which can then be exported and shared across different machines, networks, or storage devices.

Here is the detailed explanation of the different options and parameters used with the "docker save" command:

Usage: 
```
docker save [OPTIONS] IMAGE [IMAGE...]
```

OPTIONS:
```
--output, -o                  Write to a file, instead of STDOUT
```

Arguments:
```
IMAGE                         The image(s) to save to a TAR file
```

To use the "docker save" command, you need to specify the names or IDs of the Docker images that you want to archive. You can specify multiple images separated by spaces.

Example:
```
docker save my-image > my-image.tar
```

This command will save the Docker image named "my-image" to a TAR file called "my-image.tar". If you want to save multiple images, you can specify their names separated by spaces in the same command.

You can also use the "-o" or "--output" option to specify the name and location of the output file. Here's an example:
```
docker save my-image1 my-image2 -o my-images.tar
```

In this example, the Docker images "my-image1" and "my-image2" will be saved to a single TAR file called "my-images.tar".

Overall, the "docker save" command is a useful tool for anyone who wants to backup or share their Docker images. 

## tldr 
 
> Export one or more docker images to archive.
> More information: <https://docs.docker.com/engine/reference/commandline/save/>.

- Save an image by redirecting `stdout` to a tar archive:

`docker save {{image}}:{{tag}} > {{path/to/file.tar}}`

- Save an image to a tar archive:

`docker save --output {{path/to/file.tar}} {{image}}:{{tag}}`

- Save all tags of the image:

`docker save --output {{path/to/file.tar}} {{image_name}}`

- Cherry-pick particular tags of an image to save:

`docker save --output {{path/to/file.tar}} {{image_name:tag1 image_name:tag2 ...}}`
