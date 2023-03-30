# woeusb 
## chatgpt 
woeusb is a command-line utility in Linux for creating bootable Windows USB drives. It is used to create bootable Windows installation USB drives for use in installing Windows on a new or existing computer. With woeusb, you can create a bootable USB drive from a Windows ISO file or installation DVD, making it easier to install Windows on multiple computers without having to use separate DVDs or CDs.

The basic syntax for using woeusb is:

woeusb [options] source destination

Here, "source" refers to the path to the Windows ISO file or installation DVD, and "destination" refers to the path to the USB drive that you want to use as the bootable media.

Options for woeusb include:

- "--target-filesystem": Used to specify the filesystem of the USB drive (e.g., NTFS, FAT32, etc.)
- "--install": Used to install the Windows bootloader to the USB drive
- "--no-format": Used to skip formatting the USB drive before copying Windows files to it
- "--help": Shows the help menu for woeusb

To create a bootable Windows USB drive using woeusb, you must have the Windows ISO file or installation DVD and a USB drive with at least 8GB of storage space. Once you have these, you can use the woeusb command to create the bootable USB drive, specifying the source and destination as explained above. 

## tldr 
 
> Windows media creation tool.
> More information: <https://github.com/WoeUSB/WoeUSB>.

- Format a USB then create a bootable Windows installation drive:

`woeusb --device {{path/to/windows.iso}} {{/dev/sdX}}`

- Copy Windows files to an existing partition of a USB storage device and make it bootable, without erasing the current data:

`woeusb --partition {{path/to/windows.iso}} {{/dev/sdXN}}`
