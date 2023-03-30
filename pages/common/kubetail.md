# kubetail 
## chatgpt 
kubetail is a utility/command that allows you to tail logs from multiple Kubernetes pods as if they were one. It is a simple wrapper around the kubectl logs command.

Here's how it works:

1. kubetail takes a list of pod names as command line arguments.
2. It then runs kubectl logs -f on each specified pod in a separate terminal tab or window.
3. The output from each pod is interleaved and displayed in the terminal.

This makes it easier to monitor logs from multiple pods simultaneously and troubleshoot issues in a distributed system. The command can also be customized with flags such as the namespace, container, and tail lines option. 

## tldr 
 
> Utility to tail multiple Kubernetes pod logs at the same time.
> More information: <https://github.com/johanhaleby/kubetail>.

- Tail the logs of multiple pods (whose name starts with "my_app") in one go:

`kubetail {{my_app}}`

- Tail only a specific container from multiple pods:

`kubetail {{my_app}} -c {{my_container}}`

- To tail multiple containers from multiple pods:

`kubetail {{my_app}} -c {{my_container_1}} -c {{my_container_2}}`

- To tail multiple applications at the same time separate them by comma:

`kubetail {{my_app_1}},{{my_app_2}}`
