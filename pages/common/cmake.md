# cmake 
## chatgpt 
CMake is a cross-platform, open-source build system that helps in managing the build process of software projects. CMake simplifies the building process by generating native build files for various platforms, including Windows, Linux, and macOS. CMake is designed to work with different programming languages, including C, C++, and Java.

The cmake command is used to create build files for a CMake-based project. It takes a CMakeLists.txt file as input and generates platform-specific makefiles or build files. To use cmake, you need to create a CMakeLists.txt file that specifies a list of source files, headers, and libraries required for the project. Then you can run cmake to generate the necessary build files.

Some of the common options available with the cmake command are:

- -S: specifies the source directory where CMakeLists.txt can be found.
- -B: specifies the build directory where the platform-specific build files will be created.
- -G: specifies the platform-specific generator to use for creating the build files.

Here is an example of how to use the cmake command:

cmake -S /path/to/source/directory -B /path/to/build/directory -G "Unix Makefiles"

In this example, the -S option specifies the path to the source directory, -B option specifies the path to the build directory, and -G option specifies the generator to use for creating build files. The example uses the Unix Makefiles generator, which is suitable for Unix-based systems. After running this command, CMake will generate the necessary build files in the specified build directory, and you can use these files to build your project. 

## tldr 
 
> Cross-platform build automation system, that generates recipes for native build systems.
> More information: <https://cmake.org/cmake/help/latest/manual/cmake.1.html>.

- Generate a build recipe in the current directory with `CMakeLists.txt` from a project directory:

`cmake {{path/to/project_directory}}`

- Generate a build recipe, with build type set to `Release` with CMake variable:

`cmake {{path/to/project_directory}} -D {{CMAKE_BUILD_TYPE=Release}}`

- Use a generated recipe in a given directory to build artifacts:

`cmake --build {{path/to/build_directory}}`

- Install the build artifacts into `/usr/local/` and strip debugging symbols:

`cmake --install {{path/to/build_directory}} --strip`

- Install the build artifacts using the custom prefix for paths:

`cmake --install {{path/to/build_directory}} --strip --prefix {{path/to/directory}}`

- Run a custom build target:

`cmake --build {{path/to/build_directory}} --target {{target_name}}`
