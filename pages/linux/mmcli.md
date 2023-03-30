# mmcli 
## chatgpt 
The `mmcli` command is a Linux terminal command that is used to control and monitor mobile broadband devices. It is part of the ModemManager package, which is responsible for managing mobile broadband devices on Linux systems.

The `mmcli` command allows users to perform various tasks, such as checking the status of a mobile broadband device, sending SMS messages, configuring network settings, and more. It provides a complete set of options and commands that can be used to interact with the modem and various mobile broadband interfaces.

When executed, the `mmcli` command will display information about the available modems and mobile broadband devices on the system. This information includes the modem manufacturer, model, signal strength, network status, and other relevant details.

Overall, the `mmcli` command is a useful tool for managing and monitoring mobile broadband devices on Linux systems, especially when working in areas with unreliable network connections. 

## tldr 
 
> Control and monitor the ModemManager.
> More information: <https://www.freedesktop.org/software/ModemManager/man/latest/mmcli.1.html>.

- List SMS messages available on the modem:

`sudo mmcli --modem={{modem}} --messaging-list-sms`

- Delete a message from the modem, specifying its path:

`sudo mmcli --modem={{modem}} --messaging-delete-sms={{path/to/message_file}}`
