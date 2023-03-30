# stern 
## chatgpt 
Stern is a command-line interface tool that allows users to easily monitor multiple Kubernetes pods and containers. Here's a breakdown of the command:

Syntax: stern [OPTIONS] [POD_REGEX]

Options:
- `--all-namespaces` or `-A`: watch all namespaces
- `--tail`: number of lines from the end of the logs to show
- `--container`: specify the name of the container to show the logs for
- `--timestamps` or `-t`: display timestamps for each log line
- `--color` or `-c`: enable colorized output
- `--kubeconfig`: specify the path to the kubeconfig file
- `--version` or `-v`: display stern's version information
- `--help` or `-h`: display stern's help information

POD_REGEX is a required argument that specifies the regular expression used to select the target pods. Examples:
- `stern my-pod` will show logs for all containers in the `my-pod` pod
- `stern nginx` will show logs for all pods with names that match `nginx`
- `stern -A .` will show logs for all containers in all pods in all namespaces

Overall, stern allows users to quickly and easily monitor logs from multiple Kubernetes pods and containers in a single terminal window, with various options available to customize the experience. 

## tldr 
 
> Tail multiple pods and containers from Kubernetes.
> More information: <https://github.com/wercker/stern/>.

- Tail all pods within a current namespace:

`stern .`

- Tail all pods with a specific status:

`stern . --container-state {{running|waiting|terminated}}`

- Tail all pods that matches a given regular expression:

`stern {{pod_query}}`

- Tail matched pods from all namespaces:

`stern {{pod_query}} --all-namespaces`

- Tail matched pods from 15 minutes ago:

`stern {{pod_query}} --since {{15m}}`

- Tail matched pods with a specific label:

`stern {{pod_query}} --selector {{release=canary}}`
