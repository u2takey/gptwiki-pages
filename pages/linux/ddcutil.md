# ddcutil 
## chatgpt 
ddcutil is a command-line utility for interacting with monitors that support the Display Data Channel (DDC) and/or the MCCS (Monitor Control Command Set) protocols. These protocols are used to communicate between a computer and a monitor, allowing for control of various aspects of the monitor's settings such as brightness, contrast, and color temperature.

The ddcutil command can be used to perform various operations on a connected monitor, such as querying and modifying its settings. The utility supports a wide range of monitors and display adapters, and can be used on various operating systems including Linux, macOS, and Windows.

Here are some common uses of ddcutil:

- Querying the capabilities and settings of a connected monitor: 
    ```
    ddcutil detect
    ```
   This command lists all the monitors detected by ddcutil and their capabilities.

- Adjusting the brightness of a monitor: 
    ```
    ddcutil setvcp 10 50
    ```
   This command sets the brightness of the monitor to 50 (the valid range is usually 0-100) by sending the VCP (Video Control Panel) code 10, which is responsible for controlling the brightness.

- Adjusting the contrast of a monitor:
    ```
    ddcutil setvcp 12 80
    ```
   This command sets the contrast of the monitor to 80 (the valid range is usually 0-100) by sending the VCP code 12, which is responsible for controlling the contrast.

- Querying the current monitor settings:
    ```
    ddcutil getvcp 10
    ```
   This command gets the current value of the brightness setting by querying the monitor using the VCP code 10.

There are many other commands and options available in ddcutil, and you can find more information in the ddcutil manual page or documentation. 

## tldr 
 
> Control the settings of connected displays via DDC/CI.
> This command requires the kernel module `i2c-dev` to be loaded. See also: `modprobe`.
> More information: <https://www.ddcutil.com>.

- List all compatible displays:

`ddcutil detect`

- Change the brightness (option 0x10) of display 1 to 50%:

`ddcutil --display {{1}} setvcp {{10}} {{50}}`

- Increase the contrast (option 0x12) of display 1 by 5%:

`ddcutil -d {{1}} setvcp {{12}} {{+}} {{5}}`

- Read the settings of display 1:

`ddcutil -d {{1}} getvcp {{ALL}}`
