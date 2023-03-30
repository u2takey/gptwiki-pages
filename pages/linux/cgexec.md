# cgexec 
## chatgpt 
The "cgexec" command is a Linux utility that is used to run a command within a specific cgroup hierarchy. Cgroups—or control groups—are used to limit, allocate, and prioritize system resources (such as CPU, memory, and I/O) among different processes running on a Linux system.

The "cgexec" command starts a new process (specified by the command that follows) in the cgroup designated by the "-g" option. For example, the following command will start the "ls" command within the "mygroup" cgroup hierarchy:

```
cgexec -g memory:mygroup ls
```

This command will ensure that the "ls" command runs under the resource constraints set for the "mygroup" cgroup. By default, the "cgexec" command creates a new process group, so any child processes spawned by the command will also inherit the cgroup membership.

The "cgexec" command has several other options, including:

- "-p": Specifies the PID of the process to run in the cgroup (instead of starting a new process).
- "-t": Attaches the process to the current terminal (so it can receive input and output).
- "-a": Specifies additional cgroup hierarchies to add the process to (in addition to the one specified by "-g").
- "-f": Specifies a cgroup configuration file to use.

Overall, the "cgexec" command is a useful tool for managing system resources and ensuring that different processes are properly isolated and constrained. 

## tldr 
 
> Limit, measure, and control resources used by processes.
> Multiple cgroup types (aka controllers) exist, such as `cpu`, `memory`, etc.
> More information: <https://manned.org/cgexec>.

- Execute a process in a given cgroup with given controller:

`cgexec -g {{controller}}:{{cgroup_name}} {{process_name}}`
