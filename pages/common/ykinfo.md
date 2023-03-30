# ykinfo 
## chatgpt 
The command "ykinfo" is used to get information about YubiKey devices. YubiKey is a hardware authentication device used to provide two-factor authentication for a variety of online services such as Google, Dropbox, Github, etc.

The "ykinfo" command displays the details about the connected YubiKey device. This includes the firmware version, serial number, and other information about the device.

Usage: 

To run the "ykinfo" command, open a terminal window and type "ykinfo" followed by Enter. If a YubiKey device is connected, then the command will display information about the device. 

Examples:

1. Suppose you have connected a YubiKey device to your computer. Open the terminal window and type "ykinfo" and hit Enter. It will display:

Firmware version: 5.2.6
Serial number: 0123456
USB bus: 001
USB address: 005

This output shows the firmware version, serial number, and other details of the connected YubiKey device.

2. Another example is where if you connect multiple YubiKey devices to your computer, you can use the "--list" argument to list all the connected devices along with their details. Open the terminal window and type "ykinfo --list" and hit Enter. It will display:

Device 0: Yubikey 4
Firmware version: 4.3.4
Serial number: 0123456
USB bus: 001
USB address: 005

Device 1: Yubikey 5
Firmware version: 5.2.6
Serial number: 1234567
USB bus: 001
USB address: 004

This output shows the list of all connected YubiKey devices, their firmware version, serial numbers, and other details. 

## tldr 
 
> Get basic information from a YubiKey.
> More information: <https://developers.yubico.com/yubikey-personalization/Manuals/ykinfo.1.html>.

- Display all information from YubiKey:

`ykinfo -a`

- Get only serial in decimal from YubiKey:

`ykinfo -s -q`

- Get capabilities from YubiKey:

`ykinfo -c`
