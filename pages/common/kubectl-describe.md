# kubectl describe 
## chatgpt 
The command "kubectl describe" is used to retrieve detailed information about Kubernetes objects such as pods, services, nodes, deployments, and more.

When using this command, you need to provide the specific object you'd like to retrieve information for. For example, if you wanted to describe a pod called "my-pod", you would enter the command "kubectl describe pod my-pod".

The "describe" command provides a variety of information about the object, including its name, namespace, labels, status, events, containers, and more. This information can be useful for troubleshooting issues and gaining insights into how your Kubernetes cluster is functioning.

Overall, the "kubectl describe" command is a powerful tool for gaining a deeper understanding of the components that make up your Kubernetes application. 

## tldr 
 
> Show details of Kubernetes objects and resources.
> More information: <https://kubernetes.io/docs/reference/generated/kubectl/kubectl-commands#describe>.

- Show details of pods in a namespace:

`kubectl describe pods -n {{namespace}}`

- Show details of nodes in a namespace:

`kubectl describe nodes -n {{namespace}}`

- Show the details of a specific pod in a namespace:

`kubectl describe pods {{pod_name}} -n {{namespace}}`

- Show the details of a specific node in a namespace:

`kubectl describe nodes {{node_name}} -n {{namespace}}`

- Show details of Kubernetes objects defined in a YAML manifest:

`kubectl describe -f {{path/to/manifest.yaml}}`
