# sbt 
## chatgpt 
sbt stands for "Scala build tool" and is a build tool for Scala projects. It is used to manage dependencies, compile code, run tests, and package the project into a distributable artifact.

When you enter the command "sbt" on the command line, it launches the sbt shell, which allows you to interact with the tool and execute various tasks. The sbt shell provides a command-line interface where you can run tasks by entering the task name followed by any necessary arguments.

Some common tasks that can be executed using the sbt command are:

1. `compile`: Compiles the Scala code in the project.
2. `test`: Runs the tests in the project.
3. `package`: Creates a .jar file or other distributable artifact for the project.
4. `run`: Runs the main class in the project.

Additionally, using the sbt shell, you can also interact with the Scala REPL, add or remove project dependencies, manage project settings, manage plugins, and execute any other custom tasks defined in the project's build file. 

## tldr 
 
> Build tool for Scala and Java projects.
> More information: <https://www.scala-sbt.org/1.x/docs/>.

- Start a REPL (interactive shell):

`sbt`

- Create a new Scala project from an existing Giter8 template hosted on GitHub:

`sbt new {{scala/hello-world.g8}}`

- Compile and run all tests:

`sbt test`

- Delete all generated files in the `target` directory:

`sbt clean`

- Compile the main sources in `src/main/scala` and `src/main/java` directories:

`sbt compile`

- Use the specified version of sbt:

`sbt -sbt-version {{version}}`

- Use a specific jar file as the sbt launcher:

`sbt -sbt-jar {{path}}`

- List all sbt options:

`sbt -h`
