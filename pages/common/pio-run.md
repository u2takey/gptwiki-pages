# pio run 
## chatgpt 
"pio run" is a command that is commonly used in PlatformIO, an open-source ecosystem for IoT development. This command is used to compile and build a project located in the current working directory or in the project directory specified by the user. 

When "pio run" command is executed, PlatformIO first checks if the project has been initialized correctly using "pio init". If not, the user will be prompted to set up the project.

PlatformIO then goes through the process of compiling the source files and creating a binary executable file that can be uploaded to the target device. It uses the build configurations specified in the platformio.ini file to determine which toolchain and libraries to use for the build process.

If the build process is successful, the binary file will be generated in the ".pio/build/[board]/" directory, where [board] represents the target board that was specified in platformio.ini file.

Overall, "pio run" is a command that helps the user to compile and build the project for their target board, generating the binary executable required for further development. 

## tldr 
 
> Run PlatformIO project targets.
> More information: <https://docs.platformio.org/en/latest/core/userguide/cmd_run.html>.

- List all available project targets:

`pio run --list-targets`

- List all available project targets of a specific environment:

`pio run --list-targets --environment {{environment}}`

- Run all targets:

`pio run`

- Run all targets of specified environments:

`pio run --environment {{environment1}} --environment {{environment2}}`

- Run specified targets:

`pio run --target {{target1}} --target {{target2}}`

- Run the targets of a specified configuration file:

`pio run --project-conf {{path/to/platformio.ini}}`
