# fastboot 
## chatgpt 
Fastboot is a protocol and tool used to communicate with and manipulate an Android device’s bootloader ( the low-level software that loads the operating system) from a computer over USB. The fastboot command is a tool that is included with the Android software development kit (SDK) package, which is used to unlock and flash/reprogram partitions on an Android device using a computer. 

The fastboot command offers various options to communicate with and control the device's bootloader. Some of the common options available with fastboot command include:

1. Flashing boot image: This option allows you to flash a new kernel or bootloader image to your device.

2. Erase partition: This option allows you to erase an existing partition on your device.

3. Reboot device: This option reboots your device.

4. Boot device into recovery mode: This option boots the device into recovery mode.

5. Unlocking the bootloader: This option enables you to unlock the bootloader of your device, which is necessary to install custom ROMs, recoveries, and kernels.

Overall, fastboot is a powerful tool that helps Android developers and users manipulate and customize their Android devices at a low level, unlocking bootloader and other functions that may not be directly accessible from the device's user interface. 

## tldr 
 
> Communicate with connected Android devices when in bootloader mode (the one place `adb` doesn't work).
> More information: <https://cs.android.com/android/platform/superproject/+/master:system/core/fastboot>.

- Unlock the bootloader:

`fastboot oem unlock`

- Relock the bootloader:

`fastboot oem lock`

- Reboot the device from fastboot mode into fastboot mode again:

`fastboot reboot bootloader`

- Flash a given image:

`fastboot flash {{file.img}}`

- Flash a custom recovery image:

`fastboot flash recovery {{file.img}}`

- Display connected devices:

`fastboot devices`

- Display all information of a device:

`fastboot getvar all`
