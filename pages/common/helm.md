# helm 
## chatgpt 
Helm is a package manager for Kubernetes that helps to manage, deploy, and upgrade applications on a Kubernetes cluster. Helm maintains a collection of pre-packaged and versioned applications (known as charts) that you can use to manage your Kubernetes applications. With Helm, you can package all the manifests, files, and other resources required for your application and install or upgrade it with a single command.

Here are some commonly used Helm command examples:

- `helm search repo <chart>` - searches the Helm chart repository for the specified chart.
- `helm install <chart>` - installs the specified chart on the Kubernetes cluster.
- `helm upgrade <chart>` - upgrades the specified chart to the latest version on the Kubernetes cluster.
- `helm rollback <chart>` - rolls back the specified chart to a previous version if an upgrade causes issues.
- `helm list` - lists all the charts installed on the Kubernetes cluster.
- `helm delete <chart>` - uninstalls the specified chart from the Kubernetes cluster.

Overall, Helm makes it easier to deploy, manage, and upgrade applications in a Kubernetes environment. 

## tldr 
 
> Helm is a package manager for Kubernetes.
> Some subcommands such as `helm install` have their own usage documentation.
> More information: <https://helm.sh/>.

- Create a helm chart:

`helm create {{chart_name}}`

- Add a new helm repository:

`helm repo add {{repository_name}}`

- List helm repositories:

`helm repo list`

- Update helm repositories:

`helm repo update`

- Delete a helm repository:

`helm repo remove {{repository_name}}`

- Install a helm chart:

`helm install {{name}} {{repository_name}}/{{chart_name}}`

- Download helm chart as a tar archive:

`helm get {{chart_release_name}}`

- Update helm dependencies:

`helm dependency update`
