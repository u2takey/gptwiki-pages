# k3d 
## chatgpt 
k3d is a command-line tool for creating, managing, and deleting Kubernetes clusters. It creates a lightweight, single-node, multi-container Kubernetes cluster using Docker. 

Here are some of the useful commands in k3d:

- `k3d cluster create`: This creates a new Kubernetes cluster with the specified name and configuration. It can also include common plugins and network configurations.

- `k3d cluster list`: This lists all the existing Kubernetes clusters.

- `k3d cluster get-kubeconfig`: This fetches the Kubernetes configuration file for the specified cluster and saves it to a file.

- `k3d cluster delete`: This deletes the specified Kubernetes cluster and all its associated resources.

- `k3d node create`: This adds a new worker node to an existing Kubernetes cluster.

- `k3d registry create`: This creates a private Docker registry within the Kubernetes cluster.

- `k3d image import`: This imports a Docker image from the local system or external registry into the Kubernetes cluster.

Overall, k3d is a useful tool for quickly setting up and managing Kubernetes clusters on your local machine or testing environments. 

## tldr 
 
> Wrapper CLI to easily create k3s clusters inside Docker.
> More information: <https://k3d.io>.

- Create a cluster:

`k3d cluster create {{cluster_name}}`

- Delete a cluster:

`k3d cluster delete {{cluster_name}}`

- Create a new containerized k3s node:

`k3d node create {{node_name}}`

- Import an image from Docker into a k3d cluster:

`k3d image import {{image_name}} --cluster {{cluster_name}}`

- Create a new registry:

`k3d registry create {{registry_name}}`
