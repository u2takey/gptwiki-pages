# kubectl rollout 
## chatgpt 
The `kubectl rollout` command is used to manage rollouts of updates to Kubernetes resources, such as Deployments.

Here are some of the subcommands of `kubectl rollout`:

- `kubectl rollout status`: Checks the status of a rollout. For example, you can use `kubectl rollout status deployment/my-deployment` to check the status of a Deployment update.
- `kubectl rollout history`: Shows the revision history of a resource's rollout. For example, you can use `kubectl rollout history deployment/my-deployment` to see the revision history of a Deployment update.
- `kubectl rollout undo`: Rolls back a resource's update to a previous revision. For example, you can use `kubectl rollout undo deployment/my-deployment` to roll back a Deployment update.

In general, the `kubectl rollout` command is very useful for managing updates to Kubernetes resources in a way that minimizes downtime and risk. 

## tldr 
 
> Manage the rollout of a Kubernetes resource (deployments, daemonsets, and statefulsets).
> More information: <https://kubernetes.io/docs/reference/generated/kubectl/kubectl-commands#rollout>.

- Start a rolling restart of a resource:

`kubectl rollout restart {{resource_type}}/{{resource_name}}`

- Watch the rolling update status of a resource:

`kubectl rollout status {{resource_type}}/{{resource_name}}`

- Roll back a resource to the previous revision:

`kubectl rollout undo {{resource_type}}/{{resource_name}}`

- View the rollout history of a resource:

`kubectl rollout history {{resource_type}}/{{resource_name}}`
