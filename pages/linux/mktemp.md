# mktemp 
## chatgpt 
The `mktemp` command is used to create a temporary file or directory with a unique name. The name of the temporary file or directory is generated based on a template specified by the user. The template can include a string of letters, numbers, and special characters that are replaced with random characters to create a unique name.

The `mktemp` command is useful when creating temporary files or directories that are needed for a short period of time, such as when running a script or a program that requires a temporary file. Once the program has finished running, the temporary file or directory can be deleted automatically. 

The basic syntax of the `mktemp` command is:

```
mktemp [option] [template]
```

Here, `[option]` represents one or more optional command-line parameters that can be used to modify the behavior of the `mktemp` command, and `[template]` represents the template used to generate the name of the temporary file.

Some common options of `mktemp` command are:

- `-d`: It creates a temporary directory instead of a file.
- `-p`: It creates a temporary file or directory in a specified directory.
- `--suffix` or `-t`: This option adds a suffix to the end of the generated name.

For example, the command `mktemp -d /tmp/example-XXXXXX` will create a temporary directory in the `/tmp` directory with a name that starts with "example-" and ends with a unique string of characters.

In summary, the `mktemp` command generates a unique filename or directory in a temporary location with a specified format, which can be used for temporary storage or execution of scripts or programs. 

## tldr 
 
> Create a temporary file or directory.
> More information: <https://www.gnu.org/software/autogen/mktemp.html>.

- Create an empty temporary file and print the absolute path to it:

`mktemp`

- Create an empty temporary file with a given suffix and print the absolute path to file:

`mktemp --suffix "{{.ext}}"`

- Create a temporary directory and print the absolute path to it:

`mktemp --directory`
