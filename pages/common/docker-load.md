# docker load 
## chatgpt 
The "docker load" command is used to load an image in tar format into Docker. 

The syntax for using this command is: 

```
docker load [OPTIONS] [TAR_FILE]
```

Here, the OPTIONS parameter can be used to specify various options while loading the image. The TAR_FILE parameter is the path to the tar file containing the Docker image that needs to be loaded.

The command performs the following actions: 

1. Reads the specified tar file containing the image.
2. Verifies the image data to ensure that it is in the correct format for Docker.
3. Loads the image into the local Docker registry.
4. Returns a message indicating that the image has been loaded successfully.

Overall, the "docker load" command is a way to import a Docker image that has been exported using the "docker save" command, effectively allowing the image to be transferred between different Docker installations. 

## tldr 
 
> Load Docker images from files or `stdin`.
> More information: <https://docs.docker.com/engine/reference/commandline/load/>.

- Load a Docker image from `stdin`:

`docker load < {{path/to/image_file.tar}}`

- Load a Docker image from a specific file:

`docker load --input {{path/to/image_file.tar}}`

- Load a Docker image from a specific file in quiet mode:

`docker load --quiet --input {{path/to/image_file.tar}}`
