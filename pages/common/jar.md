# jar 
## chatgpt 
jar is a command used in Java programming language to create, merge, or extract Java Archive files. 

The syntax of the jar command is as follows:

jar [options] [jar-file] [manifest-file] [entry-point] files/directories

Here's what each component of the syntax means:

- options: Command line arguments that modify the behavior of the jar command.
- jar-file: The name of the resulting jar file.
- manifest-file: A file that specifies the attributes of the JAR file, such as its main class.
- entry-point: The class that should be executed when the JAR file is run (if applicable).
- files/directories: The files or directories to be added to the JAR file.

Some common options that can be passed to the jar command are:

- c: Create a new JAR file.
- x: Extract the contents of a JAR file.
- t: List the contents of a JAR file.
- v: Verbosely list the contents of a JAR file.
- f: Specify the name of the output JAR file.

Here are some examples of how the jar command can be used:

1. Create a JAR file:

jar cf myJar.jar MyClass.class

This command creates a JAR file called "myJar.jar" that contains the "MyClass.class" file.

2. Extract the contents of a JAR file:

jar xf myJar.jar

This command extracts all the files from "myJar.jar" into the current directory.

3. List the contents of a JAR file:

jar tf myJar.jar

This command lists all the files in "myJar.jar".

4. Add files to an existing JAR file:

jar uf myJar.jar newfile.txt

This command adds "newfile.txt" to "myJar.jar". 

## tldr 
 
> Java applications/libraries packager.
> More information: <https://docs.oracle.com/javase/tutorial/deployment/jar/basicsindex.html>.

- Recursively archive all files in the current directory into a .jar file:

`jar cf {{file.jar}} *`

- Unzip .jar/.war file to the current directory:

`jar -xvf {{file.jar}}`

- List a .jar/.war file content:

`jar tf {{path/to/file.jar}}`

- List a .jar/.war file content with verbose output:

`jar tvf {{path/to/file.jar}}`
