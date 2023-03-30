# pio ci 
## chatgpt 
The "pio ci" command is a PlatformIO command that is used to compile and test an embedded project. 

PIO stands for PlatformIO, which is an open-source ecosystem for developing IoT and embedded systems. It provides a unified interface for managing libraries, boards, and different development platforms. 

The "ci" in the command stands for continuous integration, which is a development practice that involves regularly building and testing an application in an automated environment. 

When you run the "pio ci" command, it compiles the code for the specified firmware, detects build errors, and runs tests to validate the functionality of the code. It can also generate build artifacts and reports for further analysis. 

The command takes several arguments, including the target board, project directory, and build flag. For example, you would run "pio ci --board=<target_board> <project_directory>" to test a project for a specific board. 

Overall, the "pio ci" command is a useful tool for ensuring the quality and reliability of embedded projects in a continuous integration environment. 

## tldr 
 
> Build PlatformIO projects with an arbitrary source code structure.
> This will create a new temporary project which the source code will be copied into.
> More information: <https://docs.platformio.org/en/latest/core/userguide/cmd_ci.html>.

- Build a PlatformIO project in the default system temporary directory and delete it afterwards:

`pio ci {{path/to/project}}`

- Build a PlatformIO project and specify specific libraries:

`pio ci --lib {{path/to/library_directory}} {{path/to/project}}`

- Build a PlatformIO project and specify a specific board (`pio boards` lists all of them):

`pio ci --board {{board}} {{path/to/project}}`

- Build a PlatformIO project in a specific directory:

`pio ci --build-dir {{path/to/build_directory}} {{path/to/project}}`

- Build a PlatformIO project and don't delete the build directory:

`pio ci --keep-build-dir {{path/to/project}}`

- Build a PlatformIO project using a specific configuration file:

`pio ci --project-conf {{path/to/platformio.ini}}`
