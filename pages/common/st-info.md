# st-info 
## chatgpt 
The st-info command is a tool that is used to retrieve information about a connected STMicroelectronics device. This command can retrieve information about the device's hardware, software versions, and other various details. 

When the st-info command is executed, it displays the following information:

1. Device type: This is the type of STMicroelectronics device that is connected to the computer, such as an STM32 development board.

2. Flash size: This is the size of the device's flash memory. It is the amount of storage available for storing programs and data.

3. RAM size: This is the amount of random access memory (RAM) available on the device. RAM is used for storing data and variables during runtime.

4. Device ID: This is a unique identifier for the device that is assigned by STMicroelectronics.

5. Chip ID: This is the identifier for the STM32 chip on the device.

6. Unique ID: This is a unique identifier that is programmed into the device by the manufacturer. 

The st-info command can be useful for developers who are working with STM32 devices, as it provides valuable information about the device's capabilities and specifications. It can also be used to verify that a device is connected to the computer and communicating properly. Overall, the st-info command is a simple and effective tool for getting information about connected STMicroelectronics devices. 

## tldr 
 
> Provides information about connected STLink and STM32 devices.
> More information: <https://github.com/texane/stlink>.

- Display amount of program memory available:

`st-info --flash`

- Display amount of SRAM memory available:

`st-info --sram`

- Display summarized information of the device:

`st-info --probe`
