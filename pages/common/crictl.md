# crictl 
## chatgpt 
The "crictl" command is used for managing container runtime interfaces (CRI) in a Kubernetes cluster. It is a command-line utility that allows administrators to interact with container runtime interfaces to perform basic operations like creating, listing, and inspecting containers.

The crictl command is available in both Linux and Windows systems and can be used to manage CRI-agnostic container runtimes like Docker, CRI-O, and containerd.

Some of the most common uses of crictl include:

1. Creating a new container: The `create` command can be used to start a new container by providing an image name and container name.

2. Inspecting a container: The `inspect` command can be used to view detailed information about an existing container.

3. Listing containers: The `ps` command can be used to list all running containers.

4. Stopping a container: The `stop` command can be used to stop a running container.

5. Removing a container: The `rm` command can be used to remove a container.

Overall, crictl is a powerful tool that allows administrators to interact with container runtimes in a Kubernetes cluster easily. 

## tldr 
 
> Command-line for CRI-compatible container runtimes.
> More information: <https://github.com/kubernetes-sigs/cri-tools/blob/master/docs/crictl.md>.

- List all kubernetes pods (Ready and NotReady):

`crictl pods`

- List all containers (Running and Exited):

`crictl ps --all`

- List all images:

`crictl images`

- Print information about specific containers:

`crictl inspect {{container_id1 container_id2 ...}}`

- Open a specific shell inside a running container:

`crictl exec -it {{container_id}} {{sh}}`

- Pull a specific image from a registry:

`crictl pull {{image:tag}}`

- Print and [f]ollow logs of a specific container:

`crictl logs -f {{container_id}}`

- Remove one or more images:

`crictl rmi {{image_id1 image_id2 ...}}`
