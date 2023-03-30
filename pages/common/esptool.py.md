# esptool.py 
## chatgpt 
esptool.py is a command-line tool used for flashing firmware to ESP8266 and ESP32 chips, which are popular microcontrollers used in a variety of DIY electronics projects.

To use the esptool.py command, you will first need to install the esptool.py program on your computer. Once installed, you will typically use the command in the following format:

esptool.py [options] [command] [command options]

Here are some of the most common options and commands:

Options:
- -p, --port : The serial port to use for communication with the chip.
- -b, --baud : The communication baud rate.
- -R, --no-stub : Disable the use of a stub bootloader (useful for older chips).
- --before default_reset : Run additional commands before resetting the chip.
- --after hard_reset : Run additional commands after resetting the chip.

Commands:
- read_flash : Read the contents of the flash memory.
- write_flash : Write firmware to the flash memory.
- erase_flash : Erase the flash memory.

For example, if you wanted to flash a firmware file called "firmware.bin" to an ESP32 chip on the serial port /dev/ttyUSB0 with a baud rate of 115200, you could use the following command:

esptool.py --port /dev/ttyUSB0 --baud 115200 write_flash 0x00000 firmware.bin

This command would write the firmware file to the beginning of flash memory (address 0x00000) on the ESP32 chip connected to /dev/ttyUSB0 at a baud rate of 115200. 

## tldr 
 
> Bootloader utility for Espressif chips (e.g. ESP8266).
> More information: <https://docs.espressif.com/projects/esptool/en/latest/esp32/>.

- Flash a firmware file to an ESP chip with a given port and baud rate:

`sudo esptool.py --port {{port}} --baud {{baud_rate}} write_flash 0x0 {{path/to/firmware.bin}}`

- Clear the flash of an ESP chip:

`sudo esptool.py --port {{port}} --baud {{baud_rate}} erase_flash`
