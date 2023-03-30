# ninja 
## chatgpt 
The "ninja" command is a build automation tool that is used to compile and build software projects. It is a lightweight and fast tool that generates build files (called "ninja files") specifically designed to work efficiently with large projects. 

When executing "ninja" command, it searches for a build file (called "build.ninja") in the current directory, and then starts building the targets specified in this file. It uses a parallel build system to execute multiple build commands at the same time, making it faster than other build tools. 

Overall, "ninja" is a command-line tool that helps developers compile and build large software projects efficiently by automating the process and running the builds in parallel. 

## tldr 
 
> A Build system designed to be fast.
> More information: <https://ninja-build.org/manual.html>.

- Build in the current directory:

`ninja`

- Build a program in a given directory:

`ninja -C {{path/to/directory}}`

- Show targets (e.g. `install` and `uninstall`):

`ninja -t targets`

- Show help:

`ninja -h`
