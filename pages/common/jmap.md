# jmap 
## chatgpt 
jmap is a command-line tool provided by Oracle's Java Development Kit (JDK) that prints the memory usage by Java process, takes a heap dump, or list the JVM internal memory used by a process.

The syntax for the jmap command is:

```jmap [option] [process-id]```


Here, the "option" refers to the available options provided by the jmap command, and "process-id" refers to the Java process for which memory usage is to be analyzed.

Some of the important options used with the jmap command are:

1. `-heap`: Displays the usage of Java heap memory. This option prints a summary of the Java heap memory usage of the specified process.

2. `-histo`: Prints a histogram of the objects present in the Java heap memory. This option prints the number of objects present in the heap memory and their size.

3. `-dump`: Takes a heap dump of the Java process. This option creates a binary dump of the heap memory of the specified process in a file.

4. `-F`: Force heap dump creation even if the process is hung.

5. `-finalizerinfo`: Prints information on objects waiting for finalization.

6. `-clstats`: Prints information on class loader statistics.

Overall, jmap is a very useful tool for diagnosing memory-related issues in Java applications. It helps in identifying memory leaks or heap dump analysis to understand the root cause of application slow down or crashes. 

## tldr 
 
> Java memory map tool.
> More information: <https://docs.oracle.com/javase/7/docs/technotes/tools/share/jmap.html>.

- Print shared object mappings for a Java process (output like pmap):

`jmap {{java_pid}}`

- Print heap summary information:

`jmap -heap {{filename.jar}} {{java_pid}}`

- Print histogram of heap usage by type:

`jmap -histo {{java_pid}}`

- Dump contents of the heap into a binary file for analysis with jhat:

`jmap -dump:format=b,file={{path/to/file}} {{java_pid}}`

- Dump live objects of the heap into a binary file for analysis with jhat:

`jmap -dump:live,format=b,file={{path/to/file}} {{java_pid}}`
