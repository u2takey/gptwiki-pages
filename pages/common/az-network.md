# az network 
## chatgpt 
az network is a command in the Azure Command-Line Interface (CLI) used to manage and configure networking resources in an Azure environment. The Azure CLI is a cross-platform command-line tool used for interacting with Azure resources, allowing developers and administrators to manage, monitor, and deploy resources using code or a terminal. 

The az network command is used to manage a variety of networking-related resources such as virtual networks, subnets, network security groups, load balancers, and virtual network gateways. It allows you to create and configure networks, view network settings and resources, and troubleshoot networking issues.

Some of the commonly used sub-commands of az network are:

- az network vnet: Used to manage virtual networks and their associated resources, such as subnets, DNS servers, addresses, and peering options.
- az network nsg: Used to manage network security groups, which control inbound and outbound traffic to a virtual network.
- az network lb: Used to manage load balancers, which allow you to distribute incoming network traffic across multiple resources.
- az network vgw: Used to manage virtual network gateways, which allow you to create secure connections between on-premises sites and a virtual network.
- az network nic: Used to manage network interface cards, which allow virtual machines to communicate over a virtual network.

Overall, the az network command is an essential tool for managing network resources in an Azure environment, and it simplifies the process of networking management through a command-line interface. 

## tldr 
 
> Manage Azure Network resources.
> Part of `azure-cli`.
> More information: <https://learn.microsoft.com/cli/azure/network>.

- List network resources in a region that are used against a subscription quota:

`az network list-usages`

- List all virtual networks in a subscription:

`az network vnet list`

- Create a virtual network:

`az network vnet create --address-prefixes {{10.0.0.0/16}} --name {{vnet}} --resource_group {{group_name}} --submet-name {{subnet}} --subnet-prefixes {{10.0.0.0/24}}`

- Enable accelerated networking for a network interface card:

`az network nic update --accelerated-networking true --name {{nic}} --resource-group {{resource_group}}`
