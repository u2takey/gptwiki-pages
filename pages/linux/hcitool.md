# hcitool 
## chatgpt 
hcitool is a command-line tool to configure and manipulate Bluetooth devices in Linux. It provides several sub-commands to perform various Bluetooth-related tasks such as scanning for nearby devices, pairing with them, setting up a connection, and much more.

Here are some of the most commonly used sub-commands of hcitool:

1. scan: Scan for nearby Bluetooth devices and display their MAC addresses and names (if available).

2. info <device>: Display information about a Bluetooth device by specifying its MAC address.

3. dev: Show information about Bluetooth devices available on the system.

4. lescan: Scan for Bluetooth low energy devices.

5. name <device> [new_name]: Get or set the name of a Bluetooth device.

6. pair <device>: Pair with a Bluetooth device by specifying its MAC address.

7. cc <device>: Connect to a Bluetooth device.

8. dc <device>: Disconnect from a Bluetooth device.

Overall, hcitool allows users to interact with Bluetooth devices from the command line efficiently. It also supports automation and scripting using shell scripts. 

## tldr 
 
> Monitor, configure connections, and send special commands to Bluetooth devices.
> More information: <https://manned.org/hcitool>.

- Scan for Bluetooth devices:

`hcitool scan`

- Output the name of a device, returning its MAC address:

`hcitool name {{bdaddr}}`

- Fetch information about a remote Bluetooth device:

`hcitool info {{bdaddr}}`

- Check the link quality to a Bluetooth device:

`hcitool lq {{bdaddr}}`

- Modify the transmit power level:

`hcitool tpl {{bdaddr}} {{0|1}}`

- Display the link policy:

`hcitool lp`

- Request authentication with a specific device:

`hcitool auth {{bdaddr}}`

- Display local devices:

`hcitool dev`
