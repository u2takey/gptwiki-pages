# kubectx 
## chatgpt 
The "kubectx" command is a command-line utility tool that allows you to switch between multiple Kubernetes contexts in your CLI easily. A Kubernetes context is defined by the combination of a cluster, a user, and a namespace. It lets you interact with the Kubernetes API server of the cluster you choose using the corresponding credentials.

When you run the "kubectx" command without any arguments, it displays a list of all available contexts. You can use the arrow keys to select a context to switch to, or you can enter the number corresponding to the context you want to switch to.

Alternatively, you can use the "kubectx" command with an argument to switch directly to a specific context. For example, to switch to a context called "prod-cluster," you can run the following command: 

```
kubectx prod-cluster
```

Once you switch to a new context, all subsequent commands you run using kubectl will be executed against that context.

The "kubectx" command also supports several other options, such as displaying the current context, adding or deleting contexts, renaming contexts, or copying contexts across namespaces. You can find more information about these options in the official documentation for the "kubectx" command. 

## tldr 
 
> Utility to manage and switch between `kubectl` contexts.
> More information: <https://github.com/ahmetb/kubectx>.

- List the contexts:

`kubectx`

- Switch to a named context:

`kubectx {{name}}`

- Switch to the previous context:

`kubectx -`

- Delete a named context:

`kubectx -d {{name}}`
