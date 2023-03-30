# kubectl get 
## chatgpt 
The "kubectl get" command is used in Kubernetes to retrieve information about resources running in the cluster. When the command "kubectl get" is run, it lists all the resources of a given resource type available in the current namespace. 

For example, if the command "kubectl get pods" is run, it will list all the pods running in the current namespace. Similarly, if the command "kubectl get services" is run, it will list all the services running in the current namespace.

The "kubectl get" command also supports various filters and output formats that can be used to customize the output according to specific requirements. These filters and output formats help in retrieving specific information about the resources, such as their status, IP address, creation and modification time, namespace, labels, annotations, etc.

Overall, the "kubectl get" command is a useful tool for monitoring and troubleshooting resources running in a Kubernetes cluster. It provides quick insights into the status of resources and helps in identifying any issues or bottlenecks. 

## tldr 
 
> Get Kubernetes objects and resources.
> More information: <https://kubernetes.io/docs/reference/generated/kubectl/kubectl-commands#get>.

- Get all namespaces in the current cluster:

`kubectl get namespaces`

- Get nodes in a specified namespace:

`kubectl get nodes -n {{namespace}}`

- Get pods in a specified namespace:

`kubectl get pods -n {{namespace}}`

- Get deployments in a specified namespace:

`kubectl get deployments -n {{namespace}}`

- Get services in a specified namespace:

`kubectl get services -n {{namespace}}`

- Get all resources in a specified namespace:

`kubectl get all -n {{namespace}}`

- Get Kubernetes objects defined in a YAML manifest:

`kubectl get -f {{path/to/manifest.yaml}}`
