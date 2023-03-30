# kustomize 
## chatgpt 
Kustomize is a command-line tool for Kubernetes that provides Kubernetes Configuration Management. It allows you to customize Kubernetes resources using a declarative approach, making it easy to manage configurations for multiple deployments in different environments, such as test, staging, and production environments.

The Kustomize command generates and applies Kubernetes manifests based on your customization files, called kustomization.yaml. These YAML files define how Kubernetes resources should be configured and customized for a given environment.

The Kustomize command provides various options like build, edit, and validate to build custom Kubernetes resources, modify existing resources or validate the Kubernetes manifests.

Below are the different subcommands of Kustomize:

1. kustomize build - This command builds Kubernetes manifests for a given kustomization.yaml file.

2. kustomize edit - This command opens the generated manifests in a text editor, allowing you to manually modify the YAML files.

3. kustomize create - This command creates a new kustomization.yaml file in the current directory.

4. kustomize validate - This command validates the generated manifests and ensures they are syntactically correct and consistent with the kustomization.yaml file.

In summary, the Kustomize command is a powerful tool that simplifies the management of Kubernetes resources by allowing users to customize and manage the manifests used in different environments.  So, If you frequently modify Kubernetes manifests for different environments, Kustomize can help you do this in a simple, efficient, and organized manner. 

## tldr 
 
> Kustomize is a tool to easily deploy resources for Kubernetes.
> More information: <https://github.com/kubernetes-sigs/kustomize>.

- Create kustomization file with resources and namespace:

`kustomize create --resources {{deployment.yaml,service.yaml}} --namespace {{staging}}`

- Build kustomization file and deploy it with `kubectl`:

`kustomize build . | kubectl apply -f -`

- Set an image in the kustomization file:

`kustomize edit set image {{busybox=alpine:3.6}}`

- Search for Kubernetes resources in the current directory to be added to the kustomization file:

`kustomize create --autodetect`
