# kube-fzf 
## chatgpt 
kube-fzf is a command-line utility tool that allows users to interact with Kubernetes resources through a Fuzzy Finder interface. The command allows users to quickly search, filter, and select Kubernetes resources using a combination of keyboard shortcuts and a search bar. By typing kube-fzf in the terminal command prompt, users can access the tool's functionality. 

Once invoked, kube-fzf displays a list of available Kubernetes resources that can be interacted with. This includes resources such as pods, services, deployments, and more. Users can then use keyboard shortcuts to filter the list or directly search for specific resources using the search bar. 

Once a desired Kubernetes resource is selected, kube-fzf will display detailed information about the resource, including its status, configuration, and other metadata. From there, users can perform various actions on the selected resource, such as deleting, editing, or scaling it. 

Overall, kube-fzf provides a fast and intuitive way for users to navigate and manage Kubernetes resources from the command line, without the need for complex commands or configuration. 

## tldr 
 
> Shell commands for command-line fuzzy searching of Kubernetes Pods.
> See also `kubectl` for related commands.
> More information: <https://github.com/thecasualcoder/kube-fzf>.

- Get pod details (from current namespace):

`findpod`

- Get pod details (from all namespaces):

`findpod -a`

- Describe a pod:

`describepod`

- Tail pod logs:

`tailpod`

- Exec into a pod's container:

`execpod {{shell_command}}`

- Port-forward a pod:

`pfpod {{port_number}}`
