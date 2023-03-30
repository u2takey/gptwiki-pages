# scala 
## chatgpt 
The command "scala" is a command line tool that runs the Scala programming language interpreter or executes a Scala script. 

When the "scala" command is run with no arguments, it launches the Scala interpreter, which is an interactive shell where users can enter Scala commands and see the result of their input instantly. The Scala interpreter can be used to try out different Scala constructs, test code snippets, or develop small Scala programs.

If the "scala" command is run with one or more arguments, it will be executed as a Scala script. The first argument to the command is the path to the script file to be executed, and any additional arguments are passed to the script as its command-line arguments. Scala scripts are simply text files containing Scala code that can be executed as a batch job. 

The Scala language is an object-oriented, functional programming language that runs on the Java Virtual Machine (JVM). Scala combines the features of object-oriented and functional programming languages to provide a concise, expressive, and powerful programming language. Scala's syntax is concise and expressive, allowing developers to write more concise and readable code than in other languages like Java. 

In summary, the "scala" command is used to launch the Scala interpreter or execute Scala scripts, which are written in the Scala programming language. 

## tldr 
 
> Scala application launcher and interactive interpreter.
> More information: <https://scala-lang.org>.

- Start a REPL (interactive shell):

`scala`

- Start the interpreter with a dependency in the classpath:

`scala -classpath {{filename.jar}} {{command}}`

- Execute a Scala script:

`scala {{script.scala}}`

- Execute a `.jar` program:

`scala {{filename.jar}}`

- Execute a single Scala command in the command-line:

`scala -e {{command}}`
