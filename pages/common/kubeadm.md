# kubeadm 
## chatgpt 
Kubeadm is a command line tool used to bootstrap and manage Kubernetes clusters. It is used to setup, initialize, and upgrade a cluster, as well as manage authentication and authorization policies. The kubeadm command is generally used to perform the following operations:

1. Initialization - The kubeadm init command initializes a new Kubernetes cluster. It creates the necessary configuration files and initializes a control plane on the node where the command is run.

2. Joining nodes - The kubeadm join command is used to add new nodes to an existing Kubernetes cluster. It executes a cluster join operation and sets up the necessary configurations for the new node to participate in the cluster.

3. Upgrade - The kubeadm upgrade command is used to upgrade an existing Kubernetes cluster to a new version. It performs a series of checks to ensure that the cluster is ready for an upgrade, and then upgrades the control plane and worker nodes.

4. Reset - The kubeadm reset command is used to remove all Kubernetes configuration files and state from the node where the command is run. It can be used to remove a node from a cluster or to start over with a fresh installation.

5. Certificate management - kubeadm also provides commands to manage the certificates used by the Kubernetes cluster, including kubeadm alpha certs, kubeadm alpha certificate, and kubeadm alpha kubeconfig.

Overall, kubeadm is an essential tool for managing Kubernetes clusters, enabling administrators to easily set up and configure new clusters, add new nodes to existing clusters, and manage the entire lifecycle of their Kubernetes infrastructure. 

## tldr 
 
> Command-line interface for creating and managing Kubernetes clusters.
> More information: <https://kubernetes.io/docs/reference/setup-tools/kubeadm>.

- Create a Kubernetes master node:

`kubeadm init`

- Bootstrap a Kubernetes worker node and join it to a cluster:

`kubeadm join --token {{token}}`

- Create a new bootstrap token with a TTL of 12 hours:

`kubeadm token create --ttl {{12h0m0s}}`

- Check if the Kubernetes cluster is upgradeable and which versions are available:

`kubeadm upgrade plan`

- Upgrade Kubernetes cluster to a specified version:

`kubeadm upgrade apply {{version}}`

- View the kubeadm ConfigMap containing the cluster's configuration:

`kubeadm config view`

- Revert changes made to the host by 'kubeadm init' or 'kubeadm join':

`kubeadm reset`
