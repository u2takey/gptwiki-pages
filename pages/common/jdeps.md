# jdeps 
## chatgpt 
The jdeps command is a tool provided by Java Development Kit (JDK) that analyzes the class dependencies in Java programs. 

It can be used to determine the package-level and class-level dependencies between Java classes or JAR files. It can also be used to detect any circular dependencies or unused classes in a Java application.

The most commonly used options of the jdeps command are:

1. -s: Prints a summary of the analysis.

2. -verbose: Enables verbose output. It is useful for analyzing complex applications with many dependencies.

3. -cp: Specifies the classpath to use when analyzing the dependencies.

4. -R: Analyzes the dependencies recursively on all classes in the specified JAR files or directories.

5. -jdkinternals: Shows the dependencies on internal JDK APIs. This option is useful for identifying dependencies on APIs that may be removed or modified in future releases.

Overall, the jdeps command is a very useful tool for analyzing and managing the dependencies in Java applications. 

## tldr 
 
> Java class dependency analyzer.
> More information: <https://docs.oracle.com/en/java/javase/18/docs/specs/man/jdeps.html>.

- Analyze the dependencies of a `.jar` or `.class` file:

`jdeps {{path/to/filename.class}}`

- Print a summary of all dependencies of a specific `.jar` file:

`jdeps {{path/to/filename.jar}} -summary`

- Print all class-level dependencies of a `.jar` file:

`jdeps {{path/to/filename.jar}} -verbose`

- Output the results of the analysis in a DOT file into a specific directory:

`jdeps {{path/to/filename.jar}} -dotoutput {{path/to/directory}}`

- Display help:

`jdeps --help`
