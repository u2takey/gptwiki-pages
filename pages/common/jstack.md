# jstack 
## chatgpt 
The `jstack` command is a Java command that is used to gather Java stack traces from a Java application. It is a diagnostic tool that can be used for troubleshooting Java application issues related to thread and memory usage. It is a part of the Java Development Kit (JDK) and is accessible through the command line.

The `jstack` command prints the Java stack trace to the console or to a specified file. It can attach to a remote Java process or to an existing Java process on the local machine. 

The command usage is as follows: 

```
jstack [ options ] [ pid | executable core ]
```

Here, `options` can be used to specify additional flags such as `-l` to print lock information, `-F` to force a stack dump of a hung or unresponsive Java process, and `-m` to print native stack frames alongside Java stack frames.

`pid` is the process ID of the target Java process, or `executable core` is the name of the executable file and core file to examine.

The `jstack` command uses the Java Virtual Machine Tool Interface (JVMTI) to gather the stack traces. It can help diagnose problems such as deadlocks, thread contention, or excessive memory usage caused by thread leaks. It is a useful tool for developers and system administrators who need to investigate issues with Java-based applications. 

Overall, the `jstack` command is a crucial tool in understanding and resolving problems related to Java stack traces. 

## tldr 
 
> Java stack trace tool.
> More information: <https://manned.org/jstack>.

- Print Java stack traces for all threads in a Java process:

`jstack {{java_pid}}`

- Print mixed mode (Java/C++) stack traces for all threads in a Java process:

`jstack -m {{java_pid}}`

- Print stack traces from Java core dump:

`jstack {{/usr/bin/java}} {{file.core}}`
