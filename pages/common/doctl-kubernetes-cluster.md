# doctl kubernetes cluster 
## chatgpt 
The `doctl kubernetes cluster` command is a command-line interface (CLI) tool. This command is used to manage and interact with a DigitalOcean Kubernetes cluster. 

Here is a detailed explanation of the command and its components:

1. `doctl` - This is the main command that invokes the DigitalOcean CLI.

2. `kubernetes` - This is a subcommand that specifies that the `doctl` CLI is interacting with Kubernetes resources.

3. `cluster` - This is a sub-subcommand that specifies that `doctl` CLI is interacting with the Kubernetes cluster resources.

The `doctl kubernetes cluster` command can be used to perform operations like creating, managing, and deleting a Kubernetes cluster, as well as getting information about a Kubernetes cluster. 

Some common subcommands that can be used with `doctl kubernetes cluster` command include:

- `create` - This subcommand is used to create a new Kubernetes cluster in DigitalOcean.

- `delete` - This subcommand is used to delete a Kubernetes cluster from DigitalOcean.

- `get` - This subcommand is used to retrieve information about a Kubernetes cluster, like its name, status, and creation date.

Overall, the `doctl kubernetes cluster` command is a powerful tool that allows developers and operations teams to manage, create, and delete Kubernetes clusters in DigitalOcean with ease. 

## tldr 
 
> Manage Kubernetes clusters and view configuration options relating to clusters.
> More information: <https://docs.digitalocean.com/reference/doctl/reference/kubernetes/cluster/>.

- Create a Kubernetes cluster:

`doctl kubernetes cluster create --count {{3}} --region {{nyc1}} --size {{s-1vcpu-2gb}} --version {{latest}} {{cluster_name}}`

- List all Kubernetes clusters:

`doctl kubernetes cluster list`

- Fetch and save the kubeconfig:

`doctl kubernetes cluster kubeconfig save {{cluster_name}}`

- Check for available upgrades:

`doctl kubernetes cluster get-upgrades {{cluster_name}}`

- Upgrade a cluster to a new Kubernetes version:

`doctl kubernetes cluster upgrade {{cluster_name}}`

- Delete a cluster:

`doctl kubernetes cluster delete {{cluster_name}}`
