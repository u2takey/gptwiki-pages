# docker secret 
## chatgpt 
Docker secrets is a command in the Docker CLI that enables secure storage and sharing of sensitive information such as passwords, certificates, and keys across a Docker swarm cluster. 

Here are the key components of the command:

- `docker secret` - this is the initial command to start using the Docker secrets feature.

- `create` - creates a new secret.

- `list` - lists all secrets in the swarm.

- `inspect` - displays detailed information about a secret.

- `rm` - removes a secret.

- `--driver` - specifies the driver used to store the secret, which can be "file," "etcd," or "vault." The default driver is "file," which stores secrets in the Docker swarm's encrypted raft log.

- `--label` - adds a label to a secret.

- `--help` - provides additional information about the usage of the `docker secret` command.

In summary, `docker secret` is a command that allows users to create, manage, and securely share sensitive information across a Docker swarm cluster using a variety of drivers and labels. 

## tldr 
 
> Manage Docker swarm secrets.
> More information: <https://docs.docker.com/engine/reference/commandline/secret/>.

- Create a new secret from `stdin`:

`{{command}} | docker secret create {{secret_name}} -`

- Create a new secret from a file:

`docker secret create {{secret_name}} {{path/to/file}}`

- List all secrets:

`docker secret ls`

- Display detailed information on one or multiple secrets in a human friendly format:

`docker secret inspect --pretty {{secret_name1 secret_name2 ...}}`

- Remove one or more secrets:

`docker secret rm {{secret_name1 secret_name2 ...}}`
