# javadoc 
## chatgpt 
The javadoc command is a tool in Java that generates documentation for Java code. The command takes Java source files and generates standard HTML pages, which can then be viewed in a web browser.

Here's a breakdown of how to use the javadoc command:

1. Open a terminal window on your computer.

2. Navigate to the directory where your Java source files are located.

3. Type "javadoc" followed by any options or parameters you want to use.

4. Press Enter to generate the documentation.

Some common options and parameters for the javadoc command include:

- "-d [directory]": This option sets the output directory for the generated documentation. For example, "javadoc -d docs" would generate the documentation in a subdirectory called "docs".

- "-sourcepath [path]": This option specifies the path where the Java source files are located. For example, "javadoc -sourcepath src" would look for source files in a directory called "src".

- "-author": This option includes author information in the generated documentation. For example, "javadoc -author" would display information about the authors of the Java code.

- "-version": This option includes version information in the generated documentation. For example, "javadoc -version" would display the version number of the Java code.

- "-classpath [path]": This option specifies the classpath where required Java classes are located. For example, "javadoc -classpath lib" would look for required classes in a directory called "lib".

Overall, the javadoc command is a useful tool for generating documentation for Java code, and it can save time and effort when documenting large projects. 

## tldr 
 
> Generate Java API documentation in HTML format from source code.
> More information: <https://docs.oracle.com/en/java/javase/19/docs/specs/man/javadoc.html>.

- Generate documentation for Java source code and save the result in a directory:

`javadoc -d {{path/to/directory/}} {{path/to/java_source_code}}`

- Generate documentation with a specific encoding:

`javadoc -docencoding {{UTF-8}} {{path/to/java_source_code}}`

- Generate documentation excluding some packages:

`javadoc -exclude {{package_list}} {{path/to/java_source_code}}`
