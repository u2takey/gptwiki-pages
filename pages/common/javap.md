# javap 
## chatgpt 
"javap" is a command-line tool provided with the Java Development Kit (JDK) that can be used to analyze Java class files and retrieve information about them. 

When you run the "javap" command, it will display information about a given class including the class name, superclass name, implemented interfaces, fields, and methods. 

Here is an outline of the basic syntax for using the "javap" command:

```
javap [options] <class or package name>
```

Options used with javap can control and alter the format of the output produced by the command. Examples of the options include:

- `-c` - prints the disassembled bytecode of each method
- `-s` - prints the signature of each method and field
- `-verbose` - prints additional debugging information

The class or package name that is provided as an argument to the "javap" command will determine the output produced by the command.

Overall, "javap" is a helpful command-line utility for Java developers who need to learn more about Java class files to understand and debug Java code. 

## tldr 
 
> Disassemble one or more class files and list them.
> More information: <https://docs.oracle.com/en/java/javase/19/docs/specs/man/javap.html>.

- Disassemble and list a `.class` file:

`javap {{path/to/file.class}}`

- Disassemble and list multiple `.class` files:

`javap {{path/to/file1.class path/to/file2.class ...}}`

- Disassemble and list a built-in class file:

`javap java.{{package}}.{{class}}`

- Display help:

`javap -help`

- Display version:

`javap -version`
