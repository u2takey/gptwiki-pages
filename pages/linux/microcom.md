# microcom 
## chatgpt 
Microcom is a command-line tool used for communicating with devices over serial ports. 

The basic syntax for using microcom is: 

```
microcom [options] [device]
```

- Options: These are additional flags that can be used to modify the behavior of the command. For example, the `-s` flag can be used to specify the baud rate for the serial communication.
- Device: This refers to the serial port device that you want to communicate with. This can be specified as a device file, such as `/dev/ttyUSB0`, or as a symbolic link, such as `serial`.

Once you have invoked microcom with the desired options and device, you will enter into a serial console session. From here, you can type commands or send data to the device connected to the serial port. 

Some common commands that can be used in microcom include:

- `ctrl-a` followed by `x`: This exits the serial console session and returns you to the terminal prompt.
- `ctrl-a` followed by `\`: This sends a break signal to the device.
- `ctrl-a` followed by `s`: This saves data transmitted to a file.
- `ctrl-a` followed by `l`: This sends the contents of a file to the device.

Overall, microcom is a useful tool for troubleshooting and configuring devices that rely on serial communication. 

## tldr 
 
> A minimalistic terminal program, used to access remote devices via a serial, CAN or telnet connection from the console.
> More information: <https://manned.org/microcom>.

- Open a serial port using the specified baud rate:

`microcom --port {{path/to/serial_port}} --speed {{baud_rate}}`

- Establish a telnet connection to the specified host:

`microcom --telnet {{hostname}}:{{port}}`
