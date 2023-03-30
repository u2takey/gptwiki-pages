# pvecm 
## chatgpt 
pvecm is a command that is used to control the cluster manager in Proxmox Virtual Environment (PVE). The pvecm command is used for cluster-wide configuration and management of the nodes.

The pvecm command can be used to perform various operations in a Proxmox cluster. Some of the most common operations include adding and removing nodes, updating the cluster configuration, checking the status of the cluster, and managing the quorum.

Here are some examples of the pvecm command:

1. pvecm add nodename - This command is used to add a new node to the PVE cluster.

2. pvecm del nodename - This command is used to remove a node from the PVE cluster.

3. pvecm status - This command is used to check the status of the PVE cluster.

4. pvecm updatecerts - This command is used to update the SSL certificates for the PVE cluster.

5. pvecm quorum status - This command is used to check the quorum status of the PVE cluster.

In summary, the pvecm command is a powerful tool for managing a Proxmox Virtual Environment cluster. It can be used to perform various tasks related to cluster configuration, management, and monitoring. 

## tldr 
 
> Proxmox VE Cluster Manager.
> More information: <https://pve.proxmox.com/pve-docs/pvecm.1.html>.

- Add the current node to an existing cluster:

`pvecm add {{hostname_or_ip}}`

- Add a node to the cluster configuration (internal use):

`pvecm addnode {{node}}`

- Return the version of the cluster join API available on this node:

`pvecm apiver`

- Generate new cluster configuration:

`pvecm create {{clustername}}`

- Remove a node from the cluster configuration:

`pvecm delnode {{node}}`

- Display the local view of the cluster nodes:

`pvecm nodes`

- Display the local view of the cluster status:

`pvecm status`
