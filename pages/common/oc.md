# oc 
## chatgpt 
The command "oc" is a command-line interface tool used for managing and viewing OpenShift Container Platform resources. It allows you to interact with your OpenShift clusters by running various commands and options.

Here are a few common examples of how to use the "oc" command:

1. Login to an OpenShift cluster: You can use the "oc login" command to login to an OpenShift cluster by specifying the server URL, username, and password. For example: oc login https://<server-url> -u username -p password

2. Create a new project or namespace: You can use the "oc new-project" command to create a new project or namespace in OpenShift. For example: oc new-project my-project

3. Deploy an application or container: You can use the "oc new-app" command to deploy an application or container in OpenShift. You can specify the container image name, environment variables, and other options. For example: oc new-app docker.io/my-image:latest

4. View resources and logs: You can use the "oc get" command to view resources and their status in OpenShift. For example: oc get pods, deployments, services. You can also use the "oc logs" command to view logs for a particular container or pod. For example: oc logs my-pod.

Overall, the "oc" command provides numerous powerful tools for managing OpenShift clusters and containerized applications. 

## tldr 
 
> The OpenShift Container Platform CLI.
> Allows for application and container management.
> More information: <https://docs.openshift.com/container-platform/3.11/cli_reference/get_started_cli.html>.

- Log in to the OpenShift Container Platform server:

`oc login`

- Create a new project:

`oc new-project {{project_name}}`

- Switch to an existing project:

`oc project {{project_name}}`

- Add a new application to a project:

`oc new-app {{repo_url}} --name {{application}}`

- Open a remote shell session to a container:

`oc rsh {{pod_name}}`

- List pods in a project:

`oc get pods`

- Log out from the current session:

`oc logout`
