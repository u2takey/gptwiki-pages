# dvc destroy 
## chatgpt 
The `dvc destroy` command is used in the data version control (DVC) system to permanently delete the data and metadata associated with a DVC project.

This command is irreversible and should be used with caution as it will delete all the tracked files, resulting in the loss of any work done on the project. Once the `dvc destroy` command is executed, it cannot be undone, and the data will be lost forever.

Before executing this command, it is recommended to make a backup of the project and its files. 

The syntax of the `dvc destroy` command is as follows:

```
dvc destroy
```

Once executed, it will prompt a warning message asking for confirmation to proceed with the deletion of data and metadata. If confirmed, it will delete all the tracked files and metadata, removing them permanently from the local storage.

It is important to note that this command should be used only if the user is absolutely sure they need to delete all data and metadata permanently. 

## tldr 
 
> Remove all DVC files and directories from a DVC project.
> More information: <https://dvc.org/doc/command-reference/destroy>.

- Destroy the current project:

`dvc destroy`

- Force destroy the current project:

`dvc destroy --force`
