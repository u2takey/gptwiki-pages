# bluetoothctl 
## chatgpt 
bluetoothctl is the command-line tool for controlling Bluetooth devices on Linux systems. It is used to manage Bluetooth adapters and devices, as well as to connect, pair, and disconnect Bluetooth devices. Here are some of the most common functions and commands associated with bluetoothctl:

1. Turning on/off Bluetooth: 

        power on/off

    This command can be used to turn the Bluetooth adapter on or off. For example, 'power on' turns the adapter on, while 'power off' turns it off.

2. Scanning for devices:

        scan on

    This command starts scanning for nearby Bluetooth devices. The results will be displayed on the terminal.

3. Listing available devices:
    
        devices

    This command lists all the Bluetooth devices that have been discovered during the scan.

4. Pairing with a device:

        pair [device MAC address]

    This command initiates pairing with a specific Bluetooth device. You need to provide the device MAC address as an argument.

5. Connecting to a device:

        connect [device MAC address]

    This command connects to a paired Bluetooth device. You need to provide the device MAC address as an argument.

6. Disconnecting from a device:

        disconnect [device MAC address]

    This command disconnects from a connected Bluetooth device. You need to provide the device MAC address as an argument.

Overall, bluetoothctl provides an efficient and powerful way to manage Bluetooth connectivity on Linux systems from the command line. 

## tldr 
 
> Manage Bluetooth devices from the command-line.
> More information: <https://bitbucket.org/serkanp/bluetoothctl>.

- Enter the `bluetoothctl` shell:

`bluetoothctl`

- List all known devices:

`bluetoothctl devices`

- Power the Bluetooth controller on or off:

`bluetoothctl power {{on|off}}`

- Pair with a device:

`bluetoothctl pair {{mac_address}}`

- Remove a device:

`bluetoothctl remove {{mac_address}}`

- Connect to a paired device:

`bluetoothctl connect {{mac_address}}`

- Disconnect from a paired device:

`bluetoothctl disconnect {{mac_address}}`

- Display help:

`bluetoothctl help`
