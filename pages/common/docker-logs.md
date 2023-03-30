# docker logs 
## chatgpt 
The `docker logs` command is used to retrieve the logs of a specific container running on Docker. This command helps in troubleshooting the container-related issues by providing an insight into the current state of the container and its history.

The syntax of the `docker logs` command is:

```
docker logs [OPTIONS] CONTAINER_ID/CONTAINER_NAME
```

Where `OPTIONS` are additional settings that can be used to customize the output and `CONTAINER_ID/CONTAINER_NAME` is the ID or name of the container whose logs are required.

Some of the commonly used options along with the `docker logs` command are:

- `-f` or `--follow`: Outputs the logs in real-time streaming fashion. Similar to the `tail -f` command in Unix systems.
- `-n` or `--tail`: Controls the number of lines to be shown from the end of the logs.
- `--since`: Filters the logs based on the time frame provided. Only shows logs generated after the specified timestamp.
- `--until`: Filters the logs based on the time frame provided. Only shows logs generated before the specified timestamp.

In summary, the `docker logs` command is an essential tool for monitoring and troubleshooting container-related issues, providing valuable insight into a container's current state and history. 

## tldr 
 
> Print container logs.
> More information: <https://docs.docker.com/engine/reference/commandline/logs>.

- Print logs from a container:

`docker logs {{container_name}}`

- Print logs and follow them:

`docker logs -f {{container_name}}`

- Print last 5 lines:

`docker logs {{container_name}} --tail {{5}}`

- Print logs and append them with timestamps:

`docker logs -t {{container_name}}`

- Print logs from a certain point in time of container execution (i.e. 23m, 10s, 2013-01-02T13:23:37):

`docker logs {{container_name}} --until {{time}}`
