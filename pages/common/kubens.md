# kubens 
## chatgpt 
The `kubens` command is a tool in Kubernetes that allows users to switch between different namespaces within a cluster quickly. A namespace provides a way to group and isolate Kubernetes resources. It allows multiple users and teams to use the same cluster without colliding with each other.

The `kubens` command is part of the `kubectx` tool, and it allows users to switch between namespaces without having to type out the full namespace name repeatedly. It provides a faster way to navigate between various namespaces used within the cluster.

When you run the `kubens` command, it lists all the available namespaces in the cluster. You can then select a namespace from the list, and the `kubens` command sets the current namespace to the selected one.

The syntax for the `kubens` command is as follows:

```
kubens <namespace-name>
```

You can specify the namespace name as an argument when you run the `kubens` command, and it will automatically switch to the specified namespace.

In conclusion, the `kubens` command is a useful tool to quickly switch between multiple namespaces within a Kubernetes cluster. It saves time as it avoids typing long namespace names repeatedly. 

## tldr 
 
> Utility to switch between Kubernetes namespaces.
> More information: <https://github.com/ahmetb/kubectx>.

- List the namespaces:

`kubens`

- Change the active namespace:

`kubens {{name}}`

- Switch to the previous namespace:

`kubens -`
