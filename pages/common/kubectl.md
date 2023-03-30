# kubectl 
## chatgpt 
`Kubectl` (Kubernetes Control) is a command-line tool used to deploy, manage, and troubleshoot applications on Kubernetes clusters. It allows users to interact with Kubernetes API objects, including pods, services, deployments, and nodes.

Some common kubectl commands include:

- `kubectl apply`: This command is used to create or update a Kubernetes resource, such as a deployment or a service. You can specify the resource definition in a YAML or JSON file or input it directly in the command line.

- `kubectl get`: This command allows users to retrieve information about Kubernetes resources. For example, `kubectl get pods` would list all pods in the current cluster.

- `kubectl describe`: This command provides detailed information about a specific Kubernetes resource. For example, `kubectl describe pod <pod-name>` would display information about the specified pod.

- `kubectl delete`: This command is used to delete Kubernetes resources, such as pods or services. You can specify the resource name, or use a selector to delete multiple resources at once.

- `kubectl logs`: This command is used to display the logs of a specific container in a pod. For example, `kubectl logs <pod-name> -c <container-name>` would display the logs for the specified container in the specified pod.

These are just a few examples of the many commands available in kubectl. To see a list of all available commands, you can use `kubectl --help` or `kubectl <command> --help` for more detailed information about a specific command. 

## tldr 
 
> Command-line interface for running commands against Kubernetes clusters.
> Some subcommands such as `kubectl run` have their own usage documentation.
> More information: <https://kubernetes.io/docs/reference/kubectl/>.

- List information about a resource with more details:

`kubectl get {{pod|service|deployment|ingress|...}} -o wide`

- Update specified pod with the label 'unhealthy' and the value 'true':

`kubectl label pods {{name}} unhealthy=true`

- List all resources with different types:

`kubectl get all`

- Display resource (CPU/Memory/Storage) usage of nodes or pods:

`kubectl top {{pod|node}}`

- Print the address of the master and cluster services:

`kubectl cluster-info`

- Display an explanation of a specific field:

`kubectl explain {{pods.spec.containers}}`

- Print the logs for a container in a pod or specified resource:

`kubectl logs {{pod_name}}`

- Run command in an existing pod:

`kubectl exec {{pod_name}} -- {{ls /}}`
