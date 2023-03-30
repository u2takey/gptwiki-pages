# gradle 
## chatgpt 
Gradle is a build automation tool that is used to compile and build source code. When the command "gradle" is executed, it will look for a build file in the current directory (e.g. build.gradle or pom.xml) and use the instructions specified in that file to build the project.

If the build file specifies a specific task (e.g. compileJava), Gradle will execute only that task. If no task is specified, Gradle will execute the default task, which is usually to build and test the project.

Gradle can also be used to manage project dependencies, run tests, generate documentation, and perform other build-related tasks.

In summary, the "gradle" command is used to build and manage projects using the Gradle build automation tool. 

## tldr 
 
> Gradle is an open source build automation system.
> More information: <https://gradle.org>.

- Compile a package:

`gradle build`

- Exclude test task:

`gradle build -x {{test}}`

- Run in offline mode to prevent Gradle from accessing the network during builds:

`gradle build --offline`

- Clear the build directory:

`gradle clean`

- Build an Android Package (APK) in release mode:

`gradle assembleRelease`

- List the main tasks:

`gradle tasks`

- List all the tasks:

`gradle tasks --all`
