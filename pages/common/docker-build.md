# docker build 
## chatgpt 
The docker build command is used to build Docker images. It takes a Dockerfile as input and uses it to create an image. 

The basic syntax for the command is:

docker build [OPTIONS] PATH | URL | -

- [OPTIONS]: These are optional flags that can be used to customize the build process. Examples of options include "-t" to tag the image, "--no-cache" to disable caching, and "--build-arg" to pass arguments to the Dockerfile.
- PATH | URL | -: This specifies the location of the Dockerfile. It can be a local path on the host machine, a URL to a Git repository, or "-" to read from standard input.

When the command is executed, Docker reads the Dockerfile and creates an image according to the instructions in the file. Each instruction in the Dockerfile creates a new layer in the image, which can be cached to speed up subsequent builds.

Once the build is complete, Docker generates a unique image ID and tags the image with the name specified by the "-t" flag. The resulting image can then be pushed to a Docker registry or used to create containers. 

## tldr 
 
> Build an image from a Dockerfile.
> More information: <https://docs.docker.com/engine/reference/commandline/build/>.

- Build a docker image using the Dockerfile in the current directory:

`docker build .`

- Build a docker image from a Dockerfile at a specified URL:

`docker build {{github.com/creack/docker-firefox}}`

- Build a docker image and tag it:

`docker build --tag {{name:tag}} .`

- Build a docker image with no build context:

`docker build --tag {{name:tag}} - < {{Dockerfile}}`

- Do not use the cache when building the image:

`docker build --no-cache --tag {{name:tag}} .`

- Build a docker image using a specific Dockerfile:

`docker build --file {{Dockerfile}} .`

- Build with custom build-time variables:

`docker build --build-arg {{HTTP_PROXY=http://10.20.30.2:1234}} --build-arg {{FTP_PROXY=http://40.50.60.5:4567}} .`
