# pio remote 
## chatgpt 
The "pio remote" command is a command-line interface tool used in PlatformIO, a popular open source ecosystem for the development of embedded systems. This command is used to interact with remote devices that are connected to the PlatformIO Network. 

When a user runs the "pio remote" command, the user is prompted to enter the remote operation to perform such as run, test, device list, and platform list. Each operation performs a different function with the connected device. 

Here are some examples of the remote operations that can be performed using "pio remote":

1. "pio remote run" command is used to build and upload firmware to a remote device. This operation sends the compiled binary to the device and runs it.

2. "pio remote device list" command is used to get a list of all remote devices (for example, with OTA support) available for the project.

3. "pio remote platform list" command is used to get a list of all supported platforms in PlatformIO's remote environment.

In summary, "pio remote" is a command-line tool used to interact with remote devices on the PlatformIO network. It provides an easy way to upload firmware, get a list of connected devices, and much more. 

## tldr 
 
> Helper command for PlatformIO Remote Development.
> `pio remote [command]` takes the same arguments as its locally executing counterpart `pio [command]`.
> More information: <https://docs.platformio.org/en/latest/core/userguide/remote/index.html>.

- List all active Remote Agents:

`pio remote agent list`

- Start a new Remote Agent with a specific name and share it with friends:

`pio remote agent start --name {{agent_name}} --share {{example1@example.com}} --share {{example2@example.com}}`

- List devices from specified Agents (omit `--agent` to specify all Agents):

`pio remote --agent {{agent_name1}} --agent {{agent_name2}} device list`

- Connect to the serial port of a remote device:

`pio remote --agent {{agent_name}} device monitor`

- Run all targets on a specified Agent:

`pio remote --agent {{agent_name}} run`

- Update installed core packages, development platforms and global libraries on a specific Agent:

`pio remote --agent {{agent_name}} update`

- Run all tests in all environments on a specific Agent:

`pio remote --agent {{agent_name}} test`
