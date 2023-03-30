# kops 
## chatgpt 
Kops (short for Kubernetes Operations) is a command-line tool that allows users to create, deploy, and manage Kubernetes clusters on AWS (Amazon Web Services). 

Here's a breakdown of some of the main commands available through kops:

1. create cluster - this command will create a new Kubernetes cluster on AWS. It requires several flags, including specifying the number and size of worker nodes, the AWS region where the cluster will be deployed, and the cluster name.

2. update cluster - this command allows users to update the configuration of an existing Kubernetes cluster. For example, users can change the number and size of worker nodes, enable/disable certain Kubernetes features, or update the version of Kubernetes used by the cluster.

3. delete cluster - this command will delete an existing Kubernetes cluster from AWS. Note that this will also delete any resources (e.g. EC2 instances, load balancers) associated with the cluster.

4. validate cluster - this command checks the configuration of an existing Kubernetes cluster to ensure that it is properly set up and configured.

5. rolling-update cluster - this command will perform a rolling update of an existing Kubernetes cluster, upgrading each node in the cluster one at a time to a new version of Kubernetes.

Overall, kops can be a useful tool for deploying and managing Kubernetes clusters on AWS, but it does require some familiarity with Kubernetes and AWS concepts. 

## tldr 
 
> Create, destroy, upgrade and maintain Kubernetes clusters from the command-line.
> More information: <https://github.com/kubernetes/kops/>.

- Create a cluster from the configuration specification:

`kops create cluster -f {{cluster_name.yaml}}`

- Create a new ssh public key:

`kops create secret sshpublickey {{key_name}} -i {{~/.ssh/id_rsa.pub}}`

- Export the cluster configuration to the `~/.kube/config` file:

`kops export kubecfg {{cluster_name}}`

- Get the cluster configuration as YAML:

`kops get cluster {{cluster_name}} -o yaml`

- Delete a cluster:

`kops delete cluster {{cluster_name}} --yes`
