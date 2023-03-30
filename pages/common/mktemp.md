# mktemp 
## chatgpt 
The "mktemp" command is a command-line utility in Unix-like operating systems like Linux and macOS that allows the creation of temporary files or directories with unique filenames, which are guaranteed not to clash with other files or directories in the system.

The syntax of the "mktemp" command is usually as follows:

```
mktemp [OPTION] [TEMPLATE]
```

Where "OPTION" specifies various behavior options, and "TEMPLATE" is a string that follows a specific format to describe the name and location of the temporary file or directory to be created. 

By default, the "mktemp" command creates a temporary file or directory in the system's default temporary directory, which usually is "/tmp" in most Unix-like systems.

The "TEMPLATE" parameter usually has the form of a string with at least six 'X' characters, which are replaced with random characters to generate a unique filename. For example, the following command will create a unique temporary directory:

```
$ mktemp -d /tmp/tempdir.XXXXXX
```

This will create a new directory with a name similar to "/tmp/tempdir.ABC123".

There are several options available to modify the behavior of the "mktemp" command. For example, the "-u" option generates a unique filename but does not create a file, which can be useful in scripts that need to generate unique names. The "-p" option specifies the directory where the temporary file or directory should be created. The "-t" option creates a unique directory tree and returns its root path.

The "mktemp" command is often used in shell scripts and other command-line utilities that need to generate temporary files or directories without worrying about naming collisions. It is a simple yet powerful tool that allows users to work with temporary files and directories in a secure and efficient way. 

## tldr 
 
> Create a temporary file or directory.
> More information: <https://ss64.com/osx/mktemp.html>.

- Create an empty temporary file and print the absolute path to it:

`mktemp`

- Create an empty temporary file with a given suffix and print the absolute path to file:

`mktemp --suffix "{{.ext}}"`

- Create a temporary directory and print the absolute path to it:

`mktemp -d`
