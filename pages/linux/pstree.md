# pstree 
## chatgpt 
The "pstree" command is a Linux/Unix system utility that displays a hierarchical tree diagram of all the running processes on the system. 

When you run the "pstree" command from the terminal, it prints out a diagram of the root process at the top, followed by a list of all its child processes for each process. Each line in the diagram represents a process, and the indentation indicates the relationship between the child and parent processes.

The syntax of the "pstree" command is simple. Open the terminal on your Linux/Unix system and type "pstree" followed by any options or arguments. Here's an example:

```
$ pstree -p
```

In this example, the "-p" option displays the process ID of each process in the diagram.

Overall, the "pstree" command is useful for system administrators, developers, and regular users who want to visualize and analyze the processes running on their Linux/Unix system. 

## tldr 
 
> A convenient tool to show running processes as a tree.
> More information: <https://manned.org/pstree>.

- Display a tree of processes:

`pstree`

- Display a tree of processes with PIDs:

`pstree -p`

- Display all process trees rooted at processes owned by specified user:

`pstree {{user}}`
