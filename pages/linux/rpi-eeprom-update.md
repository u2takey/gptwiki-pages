# rpi-eeprom-update 
## chatgpt 
`rpi-eeprom-update` is a command for updating the firmware of Raspberry Pi's embedded EEPROM (Electrically Erasable Programmable Read-Only Memory) module. EEPROM is a type of non-volatile memory that stores small amounts of data even when power is turned off.

Updating the EEPROM firmware can be useful for improving the stability, security, and functionality of the Raspberry Pi board. Some updates may also add new features or improve compatibility with certain hardware components.

Here are some details about how to use the `rpi-eeprom-update` command:

- Before updating the EEPROM, it is recommended to backup any important data or files stored on the Raspberry Pi.
- The command should be run with root privileges, so use `sudo` before the command: `sudo rpi-eeprom-update`
- The command will check if there's a new version of the EEPROM firmware available from the Raspberry Pi Foundation server. If an update is found, it will be downloaded and installed automatically, after prompting the user to confirm.
- It's a good idea to restart the Raspberry Pi afterward to ensure the new firmware is loaded successfully.
- If you want to check the current version of the EEPROM firmware, you can use the command `sudo rpi-eeprom-update -a`.

It's important to note that updating the EEPROM firmware has some risks, as it can potentially render the Raspberry Pi board unusable if something goes wrong during the update process. Therefore, it is recommended that users follow the official Raspberry Pi documentation and take necessary precautions before performing the update. 

## tldr 
 
> Tool to update EEPROM and view other EEPROM information.
> More information: <https://www.raspberrypi.com/documentation/computers/raspberry-pi.html#rpi-eeprom-update>.

- Print information about the current raspberry pi EEPROM installed:

`sudo rpi-eeprom-update`

- Update a raspberry pi EEPROM:

`sudo rpi-eeprom-update -a`

- Cancel the pending update:

`sudo rpi-eeprom-update -r`

- Display help:

`rpi-eeprom-update -h`
