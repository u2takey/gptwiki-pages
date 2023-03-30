# st-util 
## chatgpt 
`st-util` is a command-line utility used for flashing, debugging, and programming different kinds of microcontrollers that are supported by OpenOCD (On-Chip Debugging). It is typically used alongside other tools in a development environment for embedded system development.

Basically, `st-util` initializes the debugging interface and allows the device to be flashed or programmed with new firmware. It works with a range of STMicroelectronics devices, including the STM32 family of microcontrollers, and supports both JTAG and SWD protocols for debugging.

When you run `st-util`, it starts listening for incoming connections on port 4242. You can then use a debugger or other programming tool to connect to the device and use it for development purposes.

Here are some common options and arguments for `st-util`:

- `-v`, `--verbose`: Enables verbose output to help with debugging connection issues or other problems.
- `-h`, `--help`: Displays a help message with a list of available options and arguments.
- `-p`, `--listen_port PORT`: Specifies the port number that `st-util` listens on (default is 4242).
- `-m`, `--multi-core`: Enables support for debugging multi-core devices.
- `<device-name>`: Specifies the device to connect to. This can be a serial port or other device ID depending on the debug adapter being used.

Overall, `st-util` is a powerful tool for embedded system developers who need to debug or program microcontrollers. It provides a flexible interface for communicating with a range of devices, making it a valuable part of any development toolchain. 

## tldr 
 
> Run GDB (GNU Debugger) server to interact with STM32 ARM Cortex microcontoller.
> More information: <https://github.com/texane/stlink>.

- Run GDB server on port 4500:

`st-util -p {{4500}}`

- Connect to GDB server:

`(gdb) target extended-remote {{localhost}}:{{4500}}`

- Write firmware to device:

`(gdb) load {{firmware.elf}}`
