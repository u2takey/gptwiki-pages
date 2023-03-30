# javac 
## chatgpt 
The "javac" command is a command-line utility used for compiling Java code. "javac" stands for "Java Compiler".

When you write Java code, you write it in a plain text file stored with a ".java" file extension. However, this code cannot be run directly on a computer or device. It needs to be compiled into a machine-readable format called bytecode that can be executed by the Java Virtual Machine (JVM).

The "javac" command is used to compile Java code into bytecode. It takes one or more ".java" files as input and generates corresponding ".class" files as output. These ".class" files contain the bytecode for the Java program or applet.

Here is an example of how to use the "javac" command:

```javac MyClass.java```

In this example, "MyClass.java" is the name of the Java file we want to compile. The "javac" command will compile this file and, if there are no errors, create a "MyClass.class" file in the same directory.

Some common options that can be used with the "javac" command include:

- "-d" specifies the output directory for compiled ".class" files
- "-classpath" specifies the classpath for finding dependent classes
- "-verbose" prints information about the compilation process

```javac -d bin -classpath lib MyClass.java``` 

This command will compile "MyClass.java" and output the resulting ".class" files to the "bin" directory. It also specifies a classpath that includes dependent libraries located in the "lib" directory.

In summary, the "javac" command is used to compile Java code into bytecode that can be executed by the Java Virtual Machine. It takes one or more ".java" files as input and generates corresponding ".class" files as output. There are various options that can be used to customize the compilation process. 

## tldr 
 
> Java application compiler.
> More information: <https://docs.oracle.com/en/java/javase/19/docs/specs/man/javac.html>.

- Compile a `.java` file:

`javac {{file.java}}`

- Compile several `.java` files:

`javac {{file1.java}} {{file2.java}} {{file3.java}}`

- Compile all `.java` files in current directory:

`javac {{*.java}}`

- Compile a `.java` file and place the resulting class file in a specific directory:

`javac -d {{path/to/directory}} {{file.java}}`
