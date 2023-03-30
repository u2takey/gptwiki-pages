# jhsdb 
## chatgpt 
jhsdb is a command-line tool included with the Java Development Kit (JDK) that provides a range of diagnostic and troubleshooting capabilities for Java applications. The tool can be used to perform tasks such as viewing the heap memory usage of a running Java process, analyzing thread dumps, tracing code execution, and profiling performance.

Some common commands that can be run with jhsdb include:

- jhsdb jmap: Generates a heap dump of a running Java process.
- jhsdb jstack: Prints a stack trace of a running Java process, indicating which threads are currently executing and which are blocked/suspended.
- jhsdb jinfo: Provides information about a running Java process, such as JVM version, system properties, command-line arguments, and loaded classes.
- jhsdb jstat: Monitors the state of a running Java process, tracking various performance statistics such as garbage collection activity and thread counts.
- jhsdb jcmd: Sends a diagnostic command to a running Java process, such as requesting a heap dump or forcing a garbage collection.

Overall, jhsdb is a powerful tool for diagnosing and troubleshooting issues in Java applications, and can be particularly useful for debugging performance problems or memory leaks. However, it requires some knowledge of the underlying JVM and Java development concepts in order to use effectively. 

## tldr 
 
> Attach to a Java process or launch a postmortem debugger to analyze the core dump from a crashed Java Virtual Machine.
> More information: <https://manned.org/jhsdb>.

- Print stack and locks information of a Java process:

`jhsdb jstack --pid {{pid}}`

- Open a core dump in interactive debug mode:

`jhsdb clhsdb --core {{path/to/core_dump}} --exe {{path/to/jdk/bin/java}}`

- Start a remote debug server:

`jhsdb debugd --pid {{pid}} --serverid {{optional_unique_id}}`

- Connect to a process in interactive debug mode:

`jhsdb clhsdb --pid {{pid}}`
