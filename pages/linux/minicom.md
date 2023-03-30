# minicom 
## chatgpt 
Minicom is a terminal program that allows communication between a computer and a serial communication device such as a modem or serial console. It provides a user-friendly interface for managing serial communication settings and data exchange.

To use minicom, you first need to install it on your Linux or Unix-based system using the appropriate package manager (e.g. apt-get, yum, etc.). Once installed, you can launch minicom from the command line by typing 'minicom'.

When minicom starts, you will be prompted to select the serial port that you want to use for communication. You can use the arrow keys to scroll through the available options and press enter to select.

Next, you will be taken to a configuration menu where you can set various parameters such as the baud rate, data bits, parity, stop bits, and flow control. These settings must match the settings of the device that you want to communicate with.

Once you have configured the settings, you can press 'Ctrl-A' followed by 'Z' to access the command menu. From here, you can send commands to the device or adjust the settings if needed.

To exit minicom, simply press 'Ctrl-A' followed by 'X' and confirm that you want to exit. 

## tldr 
 
> A program to communicate with the serial interface of a device.
> More information: <https://manned.org/minicom>.

- Open a given serial port:

`sudo minicom --device {{/dev/ttyUSB0}}`

- Open a given serial port with a given baud rate:

`sudo minicom --device {{/dev/ttyUSB0}} --baudrate {{115200}}`

- Enter the configuration menu before communicating with a given serial port:

`sudo minicom --device {{/dev/ttyUSB0}} --setup`
