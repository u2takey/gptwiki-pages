# argocd app 
## chatgpt 
ArgoCD is a popular open source tool used for continuous deployment and management of Kubernetes applications. The `argocd app` command is one of the many commands supported by ArgoCD, and is used to perform various operations related to managing and deploying applications.

The `argocd app` command is followed by a series of sub-commands and options that define the specific operation to be executed. Some common sub-commands include:

- `create`: Creates a new application in ArgoCD.
- `delete`: Deletes an existing application from ArgoCD.
- `get`: Retrieves details about an existing application, such as its current state, configuration, and metadata.
- `patch`: Modifies the configuration of an existing application.
- `sync`: Synchronizes an application's state with its desired state, as specified in its configuration.

In addition to these sub-commands, the `argocd app` command also supports various options for specifying the application name, Git repository, branch, and more. For example, to create a new application in ArgoCD, you might use a command like the following:

```
argocd app create my-app \
  --repo https://github.com/my-org/my-repo.git \
  --path kubernetes/manifests \
  --dest-server https://my-cluster-api.example.com \
  --dest-namespace my-namespace
```

This command creates a new application called `my-app` in ArgoCD, which uses the Git repository `my-org/my-repo.git` and the Kubernetes manifests located in the `kubernetes/manifests` directory. The application is deployed to a Kubernetes cluster at the URL `https://my-cluster-api.example.com`, in the namespace `my-namespace`. 

## tldr 
 
> Command-line interface to manage applications by Argo CD.
> More information: <https://argo-cd.readthedocs.io/en/stable/user-guide/commands/argocd_app/>.

- List applications:

`argocd app list --output {{json|yaml|wide}} `

- Get application details:

`argocd app get {{app_name}} --output {{json|yaml|wide}}`

- Deploy application internally (to the same cluster that Argo CD is running in):

`argocd app create {{app_name}} --repo {{git_repo_url}} --path {{path/to/repo}} --dest-server https://kubernetes.default.svc --dest-namespace {{ns}}`

- Delete an application:

`argocd app delete {{app_name}}`

- Enable application auto-sync:

`argocd app set {{app_name}} --sync-policy auto --auto-prune --self-heal`

- Preview app synchronization without affecting cluster:

`argocd app sync {{app_name}} --dry-run --prune`

- Show application deployment history:

`argocd app history {{app_name}} --output {{wide|id}}`

- Rollback application to a previous deployed version by history ID (deleting unexpected resources):

`argocd app rollback {{app_name}} {{history_id}} --prune`
