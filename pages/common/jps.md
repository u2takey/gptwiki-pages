# jps 
## chatgpt 
The `jps` command is a utility tool used in Java development environments that displays the list of all running Java Virtual Machines (JVMs) on a local machine. The output of the 'jps' command shows the process Id (PID) of the JVMs along with their associated human-readable names.

Syntax:

To use the `jps` command, open a command prompt (terminal) and enter the command as follows:

```
jps[options]
```

Here, `[options]` is an optional list of command-line arguments that you can use to control the output format of the `jps` command.

Some of the most common `jps` options include:

- `-q`: Quiet mode, which prints only the ID of the JVMs.
- `-m`: Prints the main class name for each JVM.
- `-l`: Prints the full package name for the main class of each JVM.
- `-v`: Prints the arguments passed to the JVM.

Example:

```
jps -mlv
```

This command will display a list of running JVMs along with their process IDs, main class names, and verbose argument lists.

Sample Output:

```
18787 Jps -Denv.class.path=...
16322 JupyterKernel -XX:+HeapDumpOnOutOfMemoryError -Xmx512m ...
1229 HRegionServer -XX:+HeapDumpOnOutOfMemoryError -Xmx8388m ...
```

Here, the first column shows the process ID of each JVM, the second column shows the main class name or recognizable launcher class, and the third column shows the optional arguments passed to the JVM. 

## tldr 
 
> Show JVM process status of current user.
> More information: <https://docs.oracle.com/en/java/javase/11/tools/jps.html>.

- List all JVM processes:

`jps`

- List all JVM processes with only PID:

`jps -q`

- Display the arguments passed to the processes:

`jps -m`

- Display the full package name of all processes:

`jps -l`

- Display the arguments passed to the JVM:

`jps -v`
