# helm install 
## chatgpt 
The helm install command is used to deploy a chart as a new release to a Kubernetes cluster. It takes the following general form:

```
helm install [RELEASE NAME] [CHART] [FLAGS]
```

- `RELEASE NAME`: The name assigned to the release, which is essentially the deployment of your Kubernetes application. It could be any alphanumeric string, but it should be unique to each deployment.
- `CHART`: The path or name of the chart you want to install. It could be a directory that contains the chart files, or it could be a name of a chart repository that has already been added using `helm repo add`.
- `FLAGS`: Optional flags that provide additional information about the installation process. For example, you can use the `--set` flag to set values for specific configurations within the chart.

The `helm install` command performs multiple tasks behind the scenes, including the following:

1. Validates the chart to ensure it's properly formatted and contains all the necessary files and metadata.
2. Generates a unique name for the release based on the input `RELEASE NAME`.
3. Builds and uploads the release to the cluster, installing all necessary Kubernetes resources (pods, services, etc.) defined in the chart.
4. Tracks the status of the release, allowing you to upgrade, rollback, or uninstall it later.

Overall, the `helm install` command is a powerful tool for automating and standardizing your Kubernetes application deployment processes. 

## tldr 
 
> Install a helm chart.
> More information: <https://helm.sh/docs/intro/using_helm/#helm-install-installing-a-package>.

- Install a helm chart:

`helm install {{name}} {{repository_name}}/{{chart_name}}`

- Install a helm chart from an unpacked chart directory:

`helm install {{name}} {{path/to/source_directory}}`

- Install a helm chart from a URL:

`helm install {{package_name}} {{https://example.com/charts/packagename-1.2.3.tgz}}`

- Install a helm chart and generate a name:

`helm install {{repository_name}}/{{chart_name}} --generate-name`

- Perform a dry run:

`helm install {{name}} {{repository_name}}/{{chart_name}} --dry-run`

- Install a helm chart with custom values:

`helm install {{name}} {{repository_name}}/{{chart_name}} --set {{parameter1}}={{value1}},{{parameter2}}={{value2}}`

- Install a helm chart passing a custom values file:

`helm install {{name}} {{repository_name}}/{{chart_name}} --values {{path/to/values.yaml}}`
