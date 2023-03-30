# pueue clean 
## chatgpt 
The `pueue clean` command is used to clean up the contents of the Pueue queue. When you use Pueue to manage your tasks, it creates several files and directories in the background for storing logs, statuses, and other information. Over time, these files can accumulate and take up significant disk space. 

The `pueue clean` command cleans up these files by deleting all completed, aborted, and failed tasks logs and statuses. However, it does not remove the output files generated by task execution, as they may contain valuable information related to debugging or troubleshooting.

To execute `pueue clean`, you need to run the following command in your terminal:

```
pueue clean
```

This will clean all completed, aborted, and failed tasks from the queue. You can also specify some optional arguments to customize the command's behavior. For instance, you can use the `--all` flag to clean all tasks, including running ones. 

``` 
pueue clean --all
```

Note that you can restore a previously deleted task using the `pueue restore <task-id>` command. 

## tldr 
 
> Remove all finished tasks from the list and clear logs.
> More information: <https://github.com/Nukesor/pueue>.

- Remove finished tasks and clear logs:

`pueue clean`

- Only clean commands that finished successfully:

`pueue clean --successful-only`