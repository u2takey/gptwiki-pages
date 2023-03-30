# kube-capacity 
## chatgpt 
Kube-capacity is a command line tool used to analyze the resource utilization and capacity of Kubernetes clusters. It provides insight into the following metrics:

1. Resource usage: Displays the total amount of CPU and memory being used by the cluster, as well as the amount used by individual nodes and pods.

2. Capacity: Displays the total capacity of CPU and memory present in the cluster, as well as the capacity of each node.

3. Pod allocation: Displays the number of pods deployed in the cluster and the maximum limit set for the same.

4. Pod density: Displays the average number of pods per node in the cluster.

Using kube-capacity is simple. Just run the command with the following syntax:

```
kube-capacity [flags]
```

The available flags include:

- `kubeconfig`: Specifies the path to the Kubernetes configuration file. By default, kube-capacity uses the configuration file located at `~/.kube/config`.

- `output`: Specifies the format in which the output is printed. The available options are `text`, `json`, and `yaml`. By default, the output is printed in text format.

- `nodes`: Specifies a comma-separated list of nodes to target for analysis. By default, kube-capacity analyzes all nodes in the cluster.

- `pods`: Specifies a comma-separated list of pods to target for analysis. By default, kube-capacity analyzes all pods in the cluster.

Kube-capacity is a useful tool for monitoring the resource usage of Kubernetes clusters and can help to identify potential capacity issues before they become critical. 

## tldr 
 
> A simple CLI that provides an overview of the resource requests, limits, and utilization in a Kubernetes cluster.
> Combine the best parts of `kubectl top` and `kubectl describe` into a CLI focused on cluster resources.
> More information: <https://github.com/robscott/kube-capacity>.

- Output a list of nodes with the total CPU and Memory resource requests and limits:

`kube-capacity`

- Include pods:

`kube-capacity -p`

- Include utilization:

`kube-capacity -u`
