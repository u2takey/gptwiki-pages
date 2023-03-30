# argocd 
## chatgpt 
ArgoCD is a command-line tool for continuous deployment and GitOps practices. The tool helps to automate software delivery through a Git repository by ensuring that the application running in the Kubernetes cluster is always in sync with the desired state.

The argocd command is a tool that is used to install, configure, and manage ArgoCD. This command can be used to install ArgoCD on a Kubernetes cluster, create and manage projects, add and manage applications, monitor the system, and upgrade the tool. The command includes a rich set of subcommands to perform various tasks and options to customize the behavior of the command.

Some of the commonly used subcommands of the argocd command are:

- `install`: Installs ArgoCD on the Kubernetes cluster
- `login`: Logs in to ArgoCD's web UI or CLI
- `proj`: Creates or updates a project in ArgoCD
- `app`: Creates or updates an application in ArgoCD
- `get`: Retrieves information about the system or resources from the Kubernetes cluster
- `monitor`: Monitors the system and provides status information
- `version`: Displays the version of ArgoCD

Overall, the argocd command is an essential tool for managing ArgoCD and automation of continuous deployment and GitOps practices. 

## tldr 
 
> Command-line interface to control a Argo CD server.
> Some subcommands such as `argocd app` have their own usage documentation.
> More information: <https://argo-cd.readthedocs.io/en/stable/user-guide/commands/argocd/>.

- Login to Argo CD server:

`argocd login --insecure --username {{user}} --password {{password}} {{argocd_server:port}}`

- List applications:

`argocd app list`
