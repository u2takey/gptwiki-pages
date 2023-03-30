# archlinux-java 
## chatgpt 
The `archlinux-java` command is a utility command in Arch Linux that helps manage Java Runtime Environments (JRE) and Development Kits (JDK) installed on the system. This command provides an interface to manage all Java versions installed on the system, set default Java version, and switch between different Java versions as needed.

When you run the `archlinux-java` command, it displays a list of all Java versions installed on the system. It also displays the currently active Java version, which is denoted by an asterisk (*) next to it. You can use the command with different options and subcommands to perform various operations related to Java on Arch Linux.

Here are some common subcommands used with `archlinux-java` command:

- `-l` or `--list`: Lists all the installed Java versions on the system.

- `-v` or `--version`: Displays the active Java version.

- `-h` or `--help`: Provides a detailed help page for the command.

- `-s` or `--set`: Sets the default Java version on the system.

- `-c` or `--get-user`: Returns the user's JAVA_HOME environment variable value.

- `-u` or `--unset`: Unsets the Java version set in the JAVA_HOME environment variable.

- `--info`: Displays information about the Java version such as vendor, implementation, etc.

- `--java-home`: Displays the value of JAVA_HOME environment variable for the active Java version.

These subcommands help you set the default Java version, check the active Java version, and switch between different Java versions installed on the system. It is important to note that the `archlinux-java` command only manages the Java versions installed using the package manager in Arch Linux. If you manually install Java versions, you may need to manage them manually outside of this command. 

## tldr 
 
> A helper script that provides functionalities for Java environments.
> More information: <https://github.com/michaellass/archlinux-java-run>.

- List installed Java environments:

`archlinux-java status`

- Set the default Java environment:

`archlinux-java set {{java_environment}}`

- Unset the default Java environment:

`archlinux-java unset`

- Set the default Java environment automatically:

`archlinux-java fix`
