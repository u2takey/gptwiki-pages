# kdeconnect-cli 
## chatgpt 
The command "kdeconnect-cli" is a command-line interface (CLI) tool for KDE Connect, a software that allows communication between different devices such as smartphones and computers. 

When executed, the "kdeconnect-cli" command lists available commands for interacting with KDE Connect. These commands include sending files and notifications, triggering events on a phone or other connected devices, and monitoring the connection status. 

Examples of how to use "kdeconnect-cli" include:

- To list all available devices that are connected to KDE Connect, use the command "kdeconnect-cli -a".
- To send a text message to a connected phone, use the command "kdeconnect-cli --send-sms <phone number> <message>".
- To trigger an event on a connected device, use the command "kdeconnect-cli -d <device ID> --ping".

Overall, "kdeconnect-cli" is a powerful tool for managing KDE Connect and interacting with connected devices from the command line. 

## tldr 
 
> KDE's Connect CLI.
> More information: <https://kdeconnect.kde.org>.

- List all devices:

`kdeconnect-cli --list-devices`

- List available (paired and reachable) devices:

`kdeconnect-cli --list-available`

- Request pairing with a specific device, specifying its ID:

`kdeconnect-cli --pair --device {{device_id}}`

- Ring a device, specifying its name:

`kdeconnect-cli --ring --name "{{device_name}}"`

- Share an URL or file with a paired device, specifying its ID:

`kdeconnect-cli --share {{url|path/to/file}} --device {{device_id}}`

- Send an SMS with an optional attachment to a specific number:

`kdeconnect-cli --name "{{device_name}}" --send-sms "{{message}}" --destination {{phone_number}} --attachment {{path/to/file}}`

- Unlock a specific device:

`kdeconnect-cli --name "{{device_name}}" --unlock`

- Simulate a key press on a specific device:

`kdeconnect-cli --name "{{device_name}}" --send-keys {{key}}`
