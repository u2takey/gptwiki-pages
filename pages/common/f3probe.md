# f3probe 
## chatgpt 
F3probe is a command-line tool used to determine the actual capacity of flash memory devices such as USB drives, memory cards, and Solid State Drives (SSD). 

To use the f3probe command, you need to first install the F3 software package, which is available for Linux and Mac operating systems. Once installed, you can connect the flash memory device to your computer and run the following command:

f3probe /dev/sdb

In this command, "/dev/sdb" represents the location of the flash memory device on your system. You may need to adjust this location if your device is located elsewhere.

When you run the f3probe command, it will scan the flash memory device and provide detailed information about its capacity, available space, and speed. It can also detect any issues with the device, such as bad blocks or other hardware problems that could affect its performance and reliability.

Overall, the f3probe command is a useful tool for verifying the capacity and health of flash memory devices, especially if you are buying a used device or suspect that your existing device may be malfunctioning. 

## tldr 
 
> Probe a block device (e.g. a flash drive or a microSD card) for counterfeit flash memory.
> See also `f3read`, `f3write`, `f3fix`.
> More information: <https://github.com/AltraMayor/f3>.

- Probe a block device:

`sudo f3probe {{path/to/block_device}}`

- Use the minimum about of RAM possible:

`sudo f3probe --min-memory {{path/to/block_device}}`

- Time disk operations:

`sudo f3probe --time-ops {{path/to/block_device}}`
