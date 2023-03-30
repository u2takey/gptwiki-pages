# java 
## chatgpt 
"java" is a command used in the terminal or command prompt to run Java programs. 

When you type "java" followed by the name of a Java program file (ending in .java), the Java Virtual Machine (JVM) will interpret and execute the code in that file. 

The command may also include various options and arguments to customize the behavior of the JVM or specify additional information needed to run the program. 

For example, you may use the "-classpath" option to specify where the JVM should look for class files used by the program, or use the "-D" option to set system properties used by the program. 

Overall, "java" is an essential command for executing Java applications and is commonly used by developers, system administrators, and other users of Java technology. 

## tldr 
 
> Java application launcher.
> More information: <https://docs.oracle.com/en/java/javase/19/docs/specs/man/java.html>.

- Execute a java `.class` file that contains a main method by using just the class name:

`java {{classname}}`

- Execute a java program and use additional third-party or user-defined classes:

`java -classpath {{path/to/classes1}}:{{path/to/classes2}}:. {{classname}}`

- Execute a `.jar` program:

`java -jar {{filename.jar}}`

- Execute a `.jar` program with debug waiting to connect on port 5005:

`java -agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=*:5005 -jar {{filename.jar}}`

- Display JDK, JRE and HotSpot versions:

`java -version`

- Display usage information for the java command:

`java -help`
