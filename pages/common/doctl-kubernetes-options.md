# doctl kubernetes options 
## chatgpt 
The command "doctl kubernetes options" is used to display the available options and command flags for the DigitalOcean Kubernetes service supported by the doctl CLI (Command Line Interface) tool.

When executed, this command displays a table of options that can be specified when creating a new Kubernetes cluster or updating an existing one. These options include information such as the name of the cluster, the number and type of worker nodes, the amount of memory and CPU available to each node, the size of the cluster, the version of Kubernetes used, and more.

In addition to displaying available options, "doctl kubernetes options" also displays command flags that can be used to customize the behavior of the command. These flags include the "--output" flag, which is used to specify the output format of the command (e.g. json, yaml, etc.), and the "--wait" flag, which is used to wait for the command to complete before returning.

Overall, "doctl kubernetes options" is a useful command for anyone who wants to know what options are available when creating or updating a Kubernetes cluster on DigitalOcean. 

## tldr 
 
> Provides values available for use with doctl's Kubernetes commands.
> More information: <https://docs.digitalocean.com/reference/doctl/reference/kubernetes/options/>.

- List regions that support Kubernetes clusters:

`doctl kubernetes options regions`

- List machine sizes that can be used in a Kubernetes cluster:

`doctl kubernetes options sizes`

- List Kubernetes versions that can be used with DigitalOcean clusters:

`doctl kubernetes options versions`
