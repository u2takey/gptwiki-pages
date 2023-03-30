# pio package 
## chatgpt 
The command "pio package" is a command used in PlatformIO, an open-source ecosystem for IoT development. The command is used to package the current project as a zip archive that contains the project source code, libraries, and build output. The command creates a compressed file with the extension ".tar.gz" that can be used to share the project with others or archive it for future use.

Syntax:

To use the command "pio package", the following syntax can be used:

```
pio package [arguments]
```

Arguments:

The command "pio package" takes several arguments, which are:

- `--build-dir`: Specifies the build directory to use.

- `--verbose`: Shows extra information about the packaging process.

- `--src-filter`: Filter sources to include in the archive.

- `--exclude`: Exclude files and directories from the archive.

- `--output-dir`: Specifies the output directory.

- `--quiet`: Suppresses most console output.

- `--interactive`: Prompts the user to make choices interactively.

Function:

The pio package command packages the current project as a zip archive. The contents of the archive include the source code, any libraries used by the project, and the build output. This command is used when you want to share or archive a project with others. The command packages everything into a single archive, which can be easily shared via email, file transfer, or other means.

Example:

```
pio package --output-dir=./archives --exclude=.git --src-filter=src tests
```

This command packages the project and writes the output to the "archives" directory. It excludes the ".git" directory and only includes files in the "src" directory and the "tests" directory. 

## tldr 
 
> Manage packages in the registry.
> Packages can only be removed within 72 hours (3 days) from the date that they are published.
> More information: <https://docs.platformio.org/en/latest/core/userguide/package/>.

- Create a package tarball from the current directory:

`pio package pack --output {{path/to/package.tar.gz}}`

- Create and publish a package tarball from the current directory:

`pio package publish`

- Publish the current directory and restrict public access to it:

`pio package publish --private`

- Publish a package:

`pio package publish {{path/to/package.tar.gz}}`

- Publish a package with a custom release date (UTC):

`pio package publish {{path/to/package.tar.gz}} --released-at "{{2021-04-08 21:15:38}}"`

- Remove all versions of a published package from the registry:

`pio package unpublish {{package_name}}`

- Remove a specific version of a published package from the registry:

`pio package unpublish {{package_name}}@{{version}}`

- Undo the removal, putting all versions or a specific version of the package back into the registry:

`pio package unpublish --undo {{package_name}}@{{version}}`
