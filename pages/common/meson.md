# meson 
## chatgpt 
Meson is a build system that uses a high-level domain-specific language (DSL) to describe software projects, their dependencies, and the compilation process. It is an open-source, cross-platform build system that aims to be fast, easy-to-use, and flexible.

The meson command is the main entry point for running the Meson build system. It is used to create and configure a build directory, generate build files, and build the project. Here are some of the most common commands used with meson:

- meson setup: This command creates a build directory and generates build files based on the project description in the meson.build file.

- meson compile: This command builds the project using the settings in the build files generated by the meson setup command.

- meson test: This command runs the test suite for the project.

- meson install: This command installs the built files into the target directory.

- meson introspect: This command prints information about the build system or a specific target.

Overall, Meson is a powerful build system that provides developers with an efficient and easy-to-use way to build and deploy their projects on different platforms. 

## tldr 
 
> SCons-like build system that uses python as a front-end language and Ninja as a building backend.
> More information: <https://mesonbuild.com>.

- Generate a C project with a given name and version:

`meson init --language={{c}} --name={{myproject}} --version={{0.1}}`

- Configure the `builddir` with default values:

`meson setup {{build_dir}}`

- Build the project:

`meson compile -C {{path/to/build_dir}}`

- Run all tests in the project:

`meson test`

- Show the help:

`meson --help`

- Show version info:

`meson --version`