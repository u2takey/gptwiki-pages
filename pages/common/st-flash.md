# st-flash 
## chatgpt 
st-flash is a command-line tool used for flashing (programming) the firmware into STM32 microcontrollers' flash memory. This tool is provided by the STMicroelectronics company and is used for programming STM32 based chips. 

The st-flash command is used as follows:

```
st-flash [OPTIONS] /PATH/TO/BINARY_FILE
```

Options:

- `--reset`: This option will reset the MCU after programming it.
- `--format`: This option specifies the input format of the binary file; options are `binary`, `ihex`, or `elf`.
- `--reset-vec`: This option specifies the address of the reset vector. If not specified, the default address will be used.
- `--flash`: This option specifies the address of the flash memory where the binary file will be programmed. If not specified, the default address will be used.
- `--debug`: This option enables debug output during programming.
- `--reset-halt`: This option specifies to halt the MCU after resetting it (only applicable with the `--reset` option).

Path to binary file:

This parameter specifies the path and name of the binary file that will be programmed on the STM32. The binary file should be in one of the formats supported by the `--format` option.

Overall, the st-flash command is a powerful tool used for programming firmware onto STM32 microcontrollers' flash memory through a command-line interface, which allows for automation or scripting of the programming process. 

## tldr 
 
> Flash binary files to STM32 ARM Cortex microcontrollers.
> More information: <https://github.com/texane/stlink>.

- Read 4096 bytes from the device starting from 0x8000000:

`st-flash read {{firmware}}.bin {{0x8000000}} {{4096}}`

- Write firmware to device starting from 0x8000000:

`st-flash write {{firmware}}.bin {{0x8000000}}`

- Erase firmware from device:

`st-flash erase`
