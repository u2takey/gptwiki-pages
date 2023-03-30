# minikube 
## chatgpt 
Minikube is a command-line tool that allows you to run a single-node Kubernetes cluster on your local machine. It is designed to make it easy for developers to test and deploy their applications in a Kubernetes environment without requiring a full-scale production cluster.

Here's a breakdown of some of the key features and functionalities of the minikube command:

1. Starting and stopping a cluster: The minikube start command is used to start a new Kubernetes cluster on your local machine. This command can be used to specify various configuration options such as the size of the VM, the Kubernetes version to use, and more. Once the cluster is started, you can use the minikube stop command to shut it down.

2. Interacting with the cluster: Once the cluster is up and running, you can interact with it using the Kubernetes command-line tool, kubectl. Minikube provides a convenient way to set up the necessary environment variables for kubectl, so you don't have to worry about configuring it manually.

3. Deploying applications: You can use minikube to deploy your applications in the local Kubernetes cluster. This is done by creating a deployment and associated service objects using kubectl. Minikube also supports other methods of deploying applications, such as Helm charts and Kubernetes manifests.

4. Monitoring the cluster: Minikube provides a dashboard that allows you to monitor the state of your local Kubernetes cluster. This dashboard displays information such as the number of pods running, CPU and memory usage, and more.

Overall, the minikube command simplifies the process of running a local Kubernetes cluster and deploying applications in it. It's a great tool for developers looking to experiment with Kubernetes without having to set up a full-scale production environment. 

## tldr 
 
> Tool to run Kubernetes locally.
> More information: <https://github.com/kubernetes/minikube>.

- Start the cluster:

`minikube start`

- Get the IP address of the cluster:

`minikube ip`

- Access a service named my_service exposed via a node port and get the URL:

`minikube service {{my_service}} --url`

- Open the Kubernetes dashboard in a browser:

`minikube dashboard`

- Stop the running cluster:

`minikube stop`

- Delete the cluster:

`minikube delete`
