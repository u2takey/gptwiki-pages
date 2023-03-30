# coursier 
## chatgpt 
Coursier is a dependency resolver and launcher for Scala applications. It helps in managing the dependencies of a Scala project and also helps in packaging and distributing the application. It is similar to Maven or Gradle but is more focused on Scala applications.

The coursier command is used to execute the coursier application. It can be used to install, update, resolve, fetch or launch dependencies of a Scala project. Some examples of the commands that can be used with coursier are:

1. install - This command is used to install a specific version of a dependency. For example, coursier install org.scalatest:scalatest_2.13:3.0.8 installs the ScalaTest library version 3.0.8.

2. update - This command is used to update the dependencies of a project to the latest version available. For example, coursier update com.example:my-project_2.13 updates all the dependencies of the my-project to the latest version.

3. resolve - This command is used to resolve the dependencies of a project and their transitive dependencies. For example, coursier resolve com.example:my-project_2.13 resolves all the dependencies of the my-project including their transitive dependencies.

4. fetch - This command is used to fetch the jar files of the dependencies of a project. For example, coursier fetch com.example:my-project_2.13 fetches all the jar files of the dependencies of the my-project.

5.launch - This command is used to launch a Scala application with its dependencies. For example, coursier launch com.example:my-project_2.13:1.0.0 --main-class com.example.Main launches the main class of the my-project with its dependencies.

Overall, coursier is a useful tool for managing dependencies of Scala projects and makes it easy to package and distribute Scala applications. 

## tldr 
 
> Application and artifact manager for the Scala language, it can install Scala applications and setup your Scala development environment.
> Some subcommands such as `install`, `launch`, `java`, `fetch`, `resolve`, `complete-dep`, etc. have their own usage documentation, accessible via `tldr cs subcommand`.
> More information: <https://get-coursier.io/docs/overview>.

- Display version:

`cs version`

- Show a list of the installed applications:

`cs list`

- Install a specific application:

`cs install {{application_name}}`

- Uninstall a specific application:

`cs uninstall {{application_name}}`

- Setup machine for the Scala development:

`cs setup`

- Update all the installed applications:

`cs update`
