# pio platform 
## chatgpt 
PIO stands for PlatformIO, which is an open-source ecosystem for IoT development. "pio platform" is a command used in the PlatformIO CLI (Command Line Interface) to manage embedded platforms. 

It allows developers to view, install, and uninstall different embedded platform packages that contain board-specific configurations and tools needed for development. These platform packages can include a range of hardware platforms, such as Arduino boards, ESP8266, Raspberry Pi, and many others that provide different features and capabilities for IoT projects.

The "pio platform" command can be used with various subcommands such as list, install, uninstall, update, and show to perform different platform-related tasks within the PlatformIO environment. For example, "pio platform list" command is used to display the list of available platform packages, and "pio platform install" command is used to install a particular platform package. 

In summary, the "pio platform" command is a useful tool for IoT developers to manage and work with embedded platforms efficiently. 

## tldr 
 
> Manage PlatformIO development platforms.
> More information: <https://docs.platformio.org/en/latest/core/userguide/platforms/>.

- List all installed development platforms:

`pio platform list`

- Search for existing development platforms:

`pio platform search {{platform}}`

- Show details about a development platform:

`pio platform show {{platform}}`

- Install a development platform:

`pio platform install {{platform}}`

- Update installed development platforms:

`pio platform update`

- Uninstall a development platform:

`pio platform uninstall {{platform}}`

- List all supported frameworks:

`pio platform frameworks`
