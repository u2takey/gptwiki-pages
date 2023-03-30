# flashrom 
## chatgpt 
Flashrom is a command-line tool for reading, writing, and verifying BIOS, firmware, or other flash memory chips. It is primarily used for upgrading or downgrading the firmware of computer motherboard and peripheral devices.

The syntax for using flashrom command is: flashrom [options] [command] [filename]

Options:
-h, --help       -  Display the help message and exit
-p, --programmer -  Select the programmer to use
-r, --read       -  Read BIOS/firmware/flash chip
-w, --write      -  Write BIOS/firmware/flash chip
-v, --verify     -  Verify BIOS/firmware/flash chip
-E, --erase      -  Erase BIOS/firmware/flash chip
-c, --chip       -  Specify the flash chip
-o, --output     -  Specify the output file name

Command:
dump - Download the configuration of a flash memory.
erase - Clear the contents of a flash memory.
flash - Write code to a flash memory.
read - Retrieve the contents of a flash memory.

Example Commands:

1. To read the contents of a flash memory, use the following command:
sudo flashrom -p programmer_name -r backup.bin

2. To write firmware to a flash memory, use the following command:
sudo flashrom -p programmer_name -w firmware.bin

3. To erase the firmware of a flash memory, use the following command:
sudo flashrom -p programmer_name -E

Note: The "--help" option can be used with any command to display the help for that particular command. 

## tldr 
 
> Read, write, verify and erase flash chips.
> More information: <https://manned.org/flashrom>.

- Probe the chip, ensuring the wiring is correct:

`flashrom --programmer {{programmer}}`

- Read flash and save it to a file:

`flashrom -p {{programmer}} --read {{path/to/file}}`

- Write a file to the flash:

`flashrom -p {{programmer}} --write {{path/to/file}}`

- Verify the flash against a file:

`flashrom -p {{programmer}} --verify {{path/to/file}}`

- Probe the chip using Raspberry Pi:

`flashrom -p {{linux_spi:dev=/dev/spidev0.0}}`
