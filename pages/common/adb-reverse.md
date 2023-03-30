# adb reverse 
## chatgpt 
`adb reverse` is a command used in Android Debug Bridge (ADB) tool to reverse proxy the device's ports to the host machine. Generally, it is used to access a service running on the device from the host machine. When `adb reverse` is executed, it creates a proxy server on the host machine, which connects to a specific port on the device.

Here is how the command works:

1. Connect the device to the host machine using the USB port.
2. Enable USB debugging on the device.
3. Open a terminal window on the host machine and type in the following command: `adb reverse <remote> <local>`.

Here, `<remote>` is the port number on the device that you want to forward to the host machine, and `<local>` is the port on the host machine that will receive the traffic.

For example, if you want to connect to a service running on the device's port 8000, you can use the following command:

`adb reverse tcp:8000 tcp:8000`

This will create a reverse proxy that forwards traffic from port 8000 on the device to port 8000 on the host machine.

Once the reverse proxy is created, you can use any client on the host machine to connect to the service on the device, as if it were running on the host machine.

It is worth noting that the `adb reverse` command only works when the device is connected to the host machine via USB. If you want to access a service running on the device over the network, you will need to use other methods like port forwarding or VPN. 

## tldr 
 
> Android Debug Bridge Reverse: reverse socket connections from an Android emulator instance or connected Android devices.
> More information: <https://developer.android.com/studio/command-line/adb>.

- List all reverse socket connections from emulators and devices:

`adb reverse --list`

- Reverse a TCP port from an emulator or device to localhost:

`adb reverse tcp:{{remote_port}} tcp:{{local_port}}`

- Remove a reverse socket connections from an emulator or device:

`adb reverse --remove tcp:{{remote_port}}`

- Remove all reverse socket connections from all emulators and devices:

`adb reverse --remove-all`
