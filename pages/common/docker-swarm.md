# docker swarm 
## chatgpt 
Docker Swarm is a native clustering and orchestration solution provided by Docker. It allows users to create and manage clusters of Docker nodes, and to deploy and scale applications across those clusters.

The command "docker swarm" is used to initialize and manage a new Docker Swarm cluster. Here is a breakdown of some of the available subcommands:

- "init": This subcommand is used to initialize a new Swarm cluster on the current Docker host. It creates a new Swarm manager node and makes the current host a member of the Swarm. This command is run only once on the initial Swarm manager node.

- "join": This subcommand is used to join an existing Swarm cluster as either a manager or worker node. It requires the Swarm join token provided by the initial Swarm manager node.

- "leave": This subcommand is used to leave the current Swarm cluster. It can be run on any Swarm node to gracefully remove itself from the cluster.

- "update": This subcommand is used to update the Swarm cluster configuration, including updating the number of replicas for a service or modifying Swarm node labels.

- "services": This subcommand is used to manage the services running on the Swarm cluster, including creating, updating, and removing services.

Overall, the "docker swarm" command provides a powerful interface for managing a Docker Swarm cluster, including adding and removing nodes, updating service configurations, and scaling applications across the cluster. 

## tldr 
 
> A container orchestration tool.
> More information: <https://docs.docker.com/engine/swarm/>.

- Initialize a swarm cluster:

`docker swarm init`

- Display the token to join a manager or a worker:

`docker swarm join-token {{worker|manager}}`

- Join a new node to the cluster:

`docker swarm join --token {{token}} {{manager_node_url:2377}}`

- Remove a worker from the swarm (run inside the worker node):

`docker swarm leave`

- Display the current CA certificate in PEM format:

`docker swarm ca`

- Rotate the current CA certificate and display the new certificate:

`docker swarm ca --rotate`

- Change the valid period for node certificates:

`docker swarm update --cert-expiry {{hours}}h{{minutes}}m{{seconds}}s`
