# raspi-config 
## chatgpt 
raspi-config is a command-line utility on Raspberry Pi operating systems that is used to configure various system settings and options, such as language and regional settings, keyboard configuration, network settings, as well as hardware options like enabling the camera or changing the boot options.

When you enter the `raspi-config` command in a terminal window on a Raspberry Pi, it launches an interactive menu that allows you to navigate and select from different options that are divided into different categories like system settings, network options, boot options, display settings, and more.

Some of the most commonly used options in raspi-config include:

- Expand Filesystem: This option allows you to expand the file system to use all available space on the SD card.
- Change User Password: This option lets you change the password for the default "pi" user account.
- Change Timezone: This option allows you to set the correct time zone for your location
- Update: This option updates the Raspberry Pi's software packages to their latest versions.
- Boot Options: This option enables you to specify whether the Raspberry Pi should boot to the command line or desktop environment.

Once you've made your selections in raspi-config, the changes are saved and applied to the system.

Overall, the raspi-config command provides an easy-to-use interface for configuring and managing different settings on a Raspberry Pi, allowing you to customize and optimize your setup to suit your specific needs. 

## tldr 
 
> An `ncurses` terminal GUI to config a Raspberry Pi.
> More information: <https://www.raspberrypi.org/documentation/computers/configuration.html>.

- Start raspi-config:

`sudo raspi-config`
