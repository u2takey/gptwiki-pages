# mvn 
## chatgpt 
mvn is a command that stands for "Maven," a build automation tool for Java-based projects. It is used to build, package, and manage dependencies for a Java project.

The command "mvn" is usually followed by arguments and options that specify the task to be performed. For example, the basic syntax for building a Maven project is:

mvn clean install

The "clean" goal deletes any files that were generated from a previous build, and the "install" goal compiles and packages the project, and then installs the package into the local repository so that it can be used as a dependency by other projects.

Other common Maven goals include "compile" (compiles the source code), "test" (runs the unit tests), "package" (creates a distributable package, such as a jar file), and "deploy" (uploads the package to a remote repository, such as Nexus or Artifactory).

Maven also supports plugins, which can be used to extend its functionality for specific tasks. These plugins are configured in the pom.xml file, which is the main configuration file for a Maven project. This file defines the project's dependencies, build settings, and plugins, among other things.

In summary, the "mvn" command is a fundamental tool used in the Java development process for building, packaging, and managing dependencies of Maven-based projects, which can significantly accelerate the process of software development. 

## tldr 
 
> Apache Maven.
> Tool for building and managing Java-based projects.
> More information: <https://maven.apache.org>.

- Compile a project:

`mvn compile`

- Compile and package the compiled code in its distributable format, such as a `jar`:

`mvn package`

- Compile and package, skipping unit tests:

`mvn package -DskipTests`

- Install the built package in local maven repository. (This will invoke the compile and package commands too):

`mvn install`

- Delete build artifacts from the target directory:

`mvn clean`

- Do a clean and then invoke the package phase:

`mvn clean package`

- Clean and then package the code with a given build profile:

`mvn clean -P{{profile}} package`

- Run a class with a main method:

`mvn exec:java -Dexec.mainClass="{{com.example.Main}}" -Dexec.args="{{arg1 arg2}}"`
