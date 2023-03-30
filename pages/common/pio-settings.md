# pio settings 
## chatgpt 
The command "pio settings" is used in PlatformIO, an open source ecosystem for IoT development. 

When executing the command "pio settings", PlatformIO will display various system variables and settings that are used in the development workflow. This includes details such as the installed toolchain and compilers, the installed frameworks and libraries, and the current configuration settings. Additionally, the command enables the user to modify specific settings using the PlatformIO configuration file (platformio.ini). 

Some of the most common use cases for the "pio settings" command include troubleshooting issues related to the development environment, customizing the toolchain and build options, and optimizing the performance of the IoT device based on the available resources.

Overall, the command "pio settings" is a useful tool for developers who are working with PlatformIO, providing insightful information on the current settings and enabling customization of the development environment to meet specific project requirements. 

## tldr 
 
> View and modify PlatformIO settings.
> More information: <https://docs.platformio.org/en/latest/core/userguide/cmd_settings.html>.

- Display the names, values and descriptions of all PlatformIO settings:

`pio settings get`

- Display the name, value and description of a specific PlatformIO setting:

`pio settings get {{setting}}`

- Set a specific setting value:

`pio settings set {{setting}} {{value}}`

- Reset the values of all modified settings to their factory defaults:

`pio settings reset`
