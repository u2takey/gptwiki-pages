# kubectl run 
## chatgpt 
The command `kubectl run` is used in Kubernetes to create a new deployment or a new job. The syntax of this command is as follows:

```
kubectl run NAME --image=IMAGE [--env="key=value"] [--port=PORT] [--replicas=REPLICAS] [--dry-run=CLIENT] [--labels=key=value] [--overrides=inline-json] [--command] [--expose] [--restart=RestartPolicy] [--serviceaccount=SERVICE_ACCOUNT] [--image-pull-policy=Policy] [--output=api-version] [--requests=resource] [--limits=resource] [--args=args] [--annotations=key=value] [--pod-running-timeout=timeout] [--stdin] [--tty]
```

Here is a detailed explanation of the various options that can be used with the `kubectl run` command:

- `NAME`: This is the name of the deployment or job that you want to create.
- `--image`: This is the name of the container image that you want to use for the deployment or job.
- `--env`: This option is used to set environment variables for the container. You can use this option multiple times to set multiple variables.
- `--port`: This option is used to specify the port on which the container will listen for incoming traffic.
- `--replicas`: This option is used to specify the number of replicas for the deployment. This option is ignored if you are creating a job.
- `--dry-run`: This option allows you to see the configuration that will be sent to the server without actually creating the deployment or job.
- `--labels`: This option is used to set labels for the deployment or job. You can use this option multiple times to set multiple labels.
- `--overrides`: This option allows you to override the values of specific fields in the YAML configuration of the deployment or job.
- `--command`: This option is used to specify the command that should be run in the container.
- `--expose`: This option is used to create a service to expose the deployment or job to other pods in the cluster.
- `--restart`: This option is used to specify the restart policy for the deployment or job. You can set it to "Always", "OnFailure" or "Never".
- `--serviceaccount`: This option is used to specify the service account that should be used for the deployment or job.
- `--image-pull-policy`: This option is used to specify the image pull policy for the container. You can set it to "Always", "IfNotPresent" or "Never".
- `--output`: This option is used to specify the output format for the command. You can set it to "yaml" or "json".
- `--requests`: This option is used to specify the resource requests for the container.
- `--limits`: This option is used to specify the resource limits for the container.
- `--args`: This option is used to specify additional command line arguments for the command that should be run in the container.
- `--annotations`: This option is used to set annotations for the deployment or job.
- `--pod-running-timeout`: This option is used to set the amount of time to wait for the pod to become running before timing out.
- `--stdin`: This option is used to enable standard input for the container.
- `--tty`: This option is used to enable a terminal interface for the container. 

## tldr 
 
> Run pods in Kubernetes. Specifies pod generator to avoid deprecation error in some K8S versions.
> More information: <https://kubernetes.io/docs/reference/generated/kubectl/kubectl-commands#run>.

- Run an nginx pod and expose port 80:

`kubectl run --generator=run-pod/v1 nginx --image=nginx --port 80`

- Run an nginx pod, setting the TEST_VAR environment variable:

`kubectl run --generator=run-pod/v1 nginx --image=nginx --env="TEST_VAR=testing"`

- Show API calls that would be made to create an nginx container:

`kubectl run --generator=run-pod/v1 nginx --image=nginx --dry-run`

- Run an Ubuntu pod interactively, never restart it, and remove it when it exits:

`kubectl run --generator=run-pod/v1 -it temp-ubuntu --image=ubuntu:20.04 --restart=Never --rm -- /bin/bash`

- Run an Ubuntu pod, overriding the default command with echo, and specifying custom arguments:

`kubectl run --generator=run-pod/v1 temp-ubuntu --image=ubuntu:20.04 --command -- echo arg1 arg2 arg3`
