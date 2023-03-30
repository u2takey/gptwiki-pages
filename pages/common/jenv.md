# jenv 
## chatgpt 
jenv is a command that is used to manage multiple versions of the Java Development Kit (JDK) on a single machine. It is a command-line tool that allows you to set the default version of Java to be used in your applications, as well as switch between different versions of the JDK depending on your needs.

The jenv command allows you to install, uninstall, and list installed versions of the JDK on your computer. You can also set the global JDK version on your machine, which will be used by default in all applications, or set a local JDK version for specific applications or projects.

To use jenv, you must first install it on your machine. Once installed, you can use the following commands:

1. jenv versions - lists all installed versions of the JDK on your machine.
2. jenv global [version] - sets the global JDK version to be used by default in all applications.
3. jenv local [version] - sets the local JDK version for a specific project or application.
4. jenv shell [version] - sets the JDK version for the current shell session.
5. jenv install [version] - installs a specific version of the JDK on your machine.
6. jenv uninstall [version] - uninstalls a specific version of the JDK from your machine.

Using jenv, you can easily manage multiple versions of the JDK and ensure that your applications are running on the correct version of Java. 

## tldr 
 
> Command-line tool to manage the "JAVA_HOME" environment variable.
> More information: <https://www.jenv.be/>.

- Add a Java version to jEnv:

`jenv add {{path/to/jdk_home}}`

- Display the current JDK version used:

`jenv version`

- Display all managed JDKs:

`jenv versions`

- Set the global JDK version:

`jenv global {{java_version}}`

- Set the JDK version for the current shell session:

`jenv shell {{java_version}}`

- Enable a jEnv plugin:

`jenv enable-plugin {{plugin_name}}`
