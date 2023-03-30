# udevadm 
## chatgpt 
udevadm is a command-line utility used to control and manage the udev service, which is a subsystem in the Linux kernel responsible for managing devices connected to the system. Here are some of the common options and subcommands in udevadm:

- info: provides detailed information about a device, such as its attributes and the rules that apply to it.
- trigger: forces udev to re-evaluate the device tree and apply new rules if necessary. This is useful if a device has been added or removed from the system.
- control: allows you to control the behavior of the udev daemon, such as changing its logging level or reloading its configuration files.
- monitor: provides a real-time stream of udev events as they occur, which can be useful for debugging or monitoring device activity.

Overall, udevadm is a powerful tool for managing devices in a Linux system and should be part of any system administrator's toolkit. 

## tldr 
 
> Linux `udev` management tool.
> More information: <https://www.freedesktop.org/software/systemd/man/udevadm>.

- Monitor all device events:

`sudo udevadm monitor`

- Print `uevents` sent out by the kernel:

`sudo udevadm monitor --kernel`

- Print device events after being processed by `udev`:

`sudo udevadm monitor --udev`

- List attributes of a device:

`sudo udevadm info --attribute-walk --path {{/dev/sda1}}`

- Reload all `udev` rules:

`sudo udevadm control --reload-rules`

- Trigger all `udev` rules to run:

`sudo udevadm trigger`
