# kotlinc 
## chatgpt 
The command "kotlinc" is used to run the Kotlin compiler. 

The Kotlin programming language is a statically typed programming language that runs on the Java Virtual Machine (JVM). The kotlinc command allows you to compile Kotlin code into bytecode that can run on the JVM.

When you run the kotlinc command without any arguments, it will launch the Kotlin compiler's REPL (Read-Eval-Print Loop) which allows you to interactively experiment with the Kotlin language.

Here is an example of how to use the kotlinc command to compile a Kotlin file named HelloWorld.kt:

1. Open your terminal or command prompt.
2. Navigate to the directory where your HelloWorld.kt file is located.
3. Run the command "kotlinc HelloWorld.kt" 
4. This will compile your Kotlin source code and produce a file named "HelloWorld.class".
5. You can now run this compiled code using the command "java HelloWorld". 

Overall, the "kotlinc" command is an essential tool for Kotlin developers as it allows them to compile their code for the JVM and execute it as a Java application. 

## tldr 
 
> Kotlin compiler.
> More information: <https://kotlinlang.org/docs/command-line.html>.

- Start a REPL (interactive shell):

`kotlinc`

- Compile a Kotlin file:

`kotlinc {{path/to/file.kt}}`

- Compile several Kotlin files:

`kotlinc {{path/to/file1.kt path/to/file2.kt ...}}`

- Execute a specific Kotlin Script file:

`kotlinc -script {{path/to/file.kts}}`

- Compile a Kotlin file into a self contained jar file with the Kotlin runtime library included:

`kotlinc {{path/to/file.kt}} -include-runtime -d {{path/to/file.jar}}`
