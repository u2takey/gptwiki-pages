# docker update 
## chatgpt 
The `docker update` command allows you to update one or more properties of a running container. This command can be used to modify a container's resources allocation or security options, among other properties.

The syntax of the command is as follows:

```
docker update [OPTIONS] CONTAINER [CONTAINER...]
```

Where:
- `[OPTIONS]` are the command options that can be used to update specific properties of the container.
- `CONTAINER` is the name or ID of the container to update.

Some of the available options for the `docker update` command are:

- `--cpu-shares=<value>`: Specify the CPU shares for the container.
- `--cpus=<value>`: Specify the number of CPUs available to the container.
- `--kernel-memory=<value>`: Specify the maximum amount of kernel memory the container can use.
- `--memory=<value>`: Specify the maximum amount of memory the container can use.
- `--memory-reservation=<value>`: Specify the minimum amount of memory the container can use.
- `--restart=<value>`: Specify the restart policy for the container.
- `--security-opt=<value>`: Specify a security option for the container.

When updating a container, it's important to note that some changes may require the container to be stopped and restarted. For example, changing the number of CPUs for a container may require the container to be stopped and restarted to apply the new setting.

Overall, the `docker update` command is used to modify running containers to better suit your specific needs or requirements. 

## tldr 
 
> Update configuration of Docker containers.
> This command is not supported for Windows containers.
> More information: <https://docs.docker.com/engine/reference/commandline/update/>.

- Update restart policy to apply when a specific container exits:

`docker update --restart={{always|no|on-failure|unless-stopped}} {{container_name}}`

- Update the policy to restart up to three times a specific container when it exits with non-zero exit status:

`docker update --restart=on-failure:3 {{container_name}}`

- Update the number of CPUs available to a specific container:

`docker update --cpus {{count}} {{container_name}}`

- Update the memory limit in [M]egabytes for a specific container:

`docker update --memory {{limit}}M {{container_name}}`

- Update the maximum number of process IDs allowed inside a specific container (use `-1` for unlimited):

`docker update --pids-limit {{count}} {{container_name}}`

- Update the amount of memory in [M]egabytes a specific container can swap to disk (use `-1` for unlimited):

`docker update --memory-swap {{limit}}M {{container_name}}`
