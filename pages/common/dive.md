# dive 
## chatgpt 
Dive is a command-line tool used for exploring a Docker image or container. 

When the command is used with an image name or ID, it analyses the image layer by layer and displays information about the Dockerfile commands that created each layer. This gives users a deeper understanding of how the image was built and what dependencies are included in it. 

Dive also shows the size and type of files in each layer, highlighting potential areas for optimization. It can also display a visual representation of the image layers as a tree structure, making it easy to see the relationships between the different layers. 

When used with a running container, Dive shows the same information for the container as it does for an image, but it also provides a summary of the container's resource usage such as CPU, memory, and network. This makes it a useful tool for understanding the runtime characteristics of a containerized application. 

Overall, Dive can be a valuable tool for developers and sysadmins who need to optimize and troubleshoot Docker images and containers. 

## tldr 
 
> A tool for exploring a Docker image, layer contents, and discovering ways to shrink it.
> More information: <https://github.com/wagoodman/dive>.

- Analyze a Docker image:

`dive {{your_image_tag}}`

- Build an image and start analyzing it:

`dive build -t {{some_tag}}`
