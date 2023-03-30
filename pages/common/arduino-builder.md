# arduino-builder 
## chatgpt 
The "arduino-builder" command runs a program that is used to compile and build Arduino source code. It is a command-line tool that can be used to build Arduino projects from the terminal/command prompt.

The arduino-builder command is typically used in conjunction with the Arduino IDE or other code editor software to automate the process of building Arduino sketches. It is also used by developers who prefer to work with command-line interfaces rather than graphical user interfaces.

When executed, the arduino-builder program takes the sketch code written in C or C++ and compiles it into a binary file that can be uploaded to the Arduino hardware. The builder program is capable of handling libraries, dependencies, and platform-specific configurations, making it ideal for building complex Arduino projects.

Overall, the arduino-builder command simplifies the process of building and uploading Arduino code to the board, making it easier for programmers to develop and test their projects more efficiently. 

## tldr 
 
> A command-line tool for compiling arduino sketches.
> DEPRECATION WARNING: This tool is being phased out in favor of `arduino`.
> More information: <https://github.com/arduino/arduino-builder>.

- Compile a sketch:

`arduino-builder -compile {{path/to/sketch.ino}}`

- Specify the debug level (default: 5):

`arduino-builder -debug-level {{1..10}}`

- Specify a custom build directory:

`arduino-builder -build-path {{path/to/build_directory}}`

- Use a build option file, instead of specifying `--hardware`, `--tools`, etc. manually every time:

`arduino-builder -build-options-file {{path/to/build.options.json}}`

- Enable verbose mode:

`arduino-builder -verbose {{true}}`
