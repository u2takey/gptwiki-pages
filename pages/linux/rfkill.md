# rfkill 
## chatgpt 
The `rfkill` command on Linux is used to query or modify the state of wireless devices like WiFi, Bluetooth, etc. that are either hardware or software blocked. The `rfkill` stands for Radio Frequency Kill.

Syntax:
```
rfkill [options] command
```

Options:
* `-e [type]`: List all devices.
* `-o [type]`: Output report in different format.
* `-I`: Import key from file.
* `-X`: Export key to file.
* `-V`: Display version of `rfkill`.

Commands:
* `list`: List all radio devices and their states.
* `event`: Display events generated by the kernel.
* `block [index]`: Block a device by index.
* `unblock [index]`: Unblock a device by index.
* `block [type]`: Block all devices of a certain type.
* `unblock [type]`: Unblock all devices of a certain type.

Example:
```
rfkill list
```

This command will list all the wireless devices, along with their block status, in a table format. It will show the following information:
* Index: ID of the wireless device.
* Type: Type of the wireless device.
* Soft blocked: Shows whether a device is blocked by software.
* Hard blocked: Shows whether a device is blocked by hardware.

Output:
```
0: phy0: Wireless LAN
        Soft blocked: no
        Hard blocked: no
```

This output shows that the wireless LAN device with index 0 is neither soft nor hard blocked. 

## tldr 
 
> Enable and disable wireless devices.
> More information: <https://manned.org/rfkill>.

- List devices:

`rfkill`

- Filter by columns:

`rfkill -o {{ID,TYPE,DEVICE}}`

- Block devices by type (e.g. bluetooth, wlan):

`rfkill block {{bluetooth}}`

- Unblock devices by type (e.g. bluetooth, wlan):

`rfkill unblock {{wlan}}`

- Output in JSON format:

`rfkill -J`