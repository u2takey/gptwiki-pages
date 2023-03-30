# rpi-imager 
## chatgpt 
rpi-imager is a graphical utility that allows you to easily create SD cards for use with Raspberry Pi devices. It is a cross-platform tool that can be used on Windows, macOS, and Linux.

Once installed, you simply select the operating system image you want to write to the card, select the card itself from a list of available devices, and press the "Write" button. The software will then format the card and write the image to it.

The rpi-imager tool can also be used to back up or clone existing Raspberry Pi images. Additionally, it provides a way to verify the integrity of the written images by comparing the hash values of the source and target files.

In summary, rpi-imager is a simple and convenient tool for managing SD cards for Raspberry Pi devices. 

## tldr 
 
> Flash images onto storage devices.
> More information: <https://github.com/raspberrypi/rpi-imager>.

- Write a specific image to a specific block device:

`rpi-imager --cli {{path/to/image.zip}} {{/dev/sdX}}`

- Write a specific image to a block device, disabling the checksum verification:

`rpi-imager --cli --disable-verify {{path/to/image.zip}} {{/dev/sdX}}`

- Write a specific image to a block device, which will expect a specific checksum when running the verification:

`rpi-imager --cli --sha256 {{expected_hash}} {{path/to/image.zip}} {{/dev/sdX}}`
