# avrdude 
## chatgpt 
avrdude is a command-line program used for uploading firmware or programs to Atmel AVR microcontrollers, which are commonly used in embedded systems. It can be used to program both the flash memory and EEPROM of AVR microcontrollers via various programming interfaces like ISP, JTAG, and UART. 

The avrdude command syntax typically includes several parameters that must be specified to specify the target microcontroller, the programming interface, and the firmware to be uploaded. For example, the basic syntax for avrdude might look like this:

```
avrdude -c programmer-name -p target-microcontroller -U flash/write/read/eeprom/etc:target-file-name.hex
```

Here's what each part of the syntax means:

- `avrdude` is the command itself.
- `-c programmer-name` specifies the programming interface to be used for communicating with the target microcontroller, such as USBasp, AVRISP, or AtmelICE.
- `-p target-microcontroller` specifies the microcontroller model to be programmed, such as ATmega328P or ATtiny85.
- `-U flash/write/read/eeprom/etc:target-file-name.hex` specifies the type of memory to be programmed (flash, EEPROM, fuse bits, etc.) and the target file name in Intel HEX format. 

In addition to these basic parameters, avrdude supports many other options and configurations for specific use cases, such as setting fuse bits, verifying the programmed firmware, specifying the communication protocol, and more. Overall, avrdude is a powerful tool for working with Atmel AVR microcontrollers and is widely used by developers and hobbyists in the embedded systems community. 

## tldr 
 
> Driver program for Atmel AVR microcontrollers programming.
> More information: <https://www.nongnu.org/avrdude/>.

- Read AVR microcontroller:

`avrdude -p {{AVR_device}} -c {{programmer}} -U flash:r:{{file.hex}}:i`

- Write AVR microcontroller:

`avrdude -p {{AVR_device}} -c {{programmer}} -U flash:w:{{file.hex}}`

- List available AVR devices:

`avrdude -p \?`

- List available AVR programmers:

`avrdude -c \?`
