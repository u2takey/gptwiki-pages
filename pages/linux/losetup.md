# losetup 
## chatgpt 
The `losetup` command is a Linux command that is used to set up and control loop devices. Loop devices are special virtual devices that allow you to map a file or block device to a regular file or directory on your system.

The `losetup` command has a variety of options and subcommands that allow you to perform different actions with loop devices. Some of the most commonly used options include:

1. `-f` or `--find`: Finds the first available loop device and sets it up.

2. `-e` or `--encryption`: Specifies the encryption algorithm to use when setting up the loop device.

3. `-r` or `--read-only`: Sets the loop device to read-only mode.

4. `-d` or `--detach`: Detaches the loop device from the file or block device it is associated with.

5. `-a` or `--show`: Displays information about all currently set up loop devices.

6. `-h` or `--help`: Displays a help message with a list of available options.

To use the `losetup` command, you typically specify the path to the file or block device you want to associate with the loop device, along with any desired options. For example, the command `losetup /dev/loop0 /path/to/file` would create a new loop device at `/dev/loop0` and associate it with the file located at `/path/to/file`. 

Overall, the `losetup` command is a powerful tool for managing loop devices in Linux systems. It can be used for a variety of tasks, such as mounting disk images, creating encrypted filesystems, and more. 

## tldr 
 
> Set up and control loop devices.
> More information: <https://manned.org/losetup>.

- List loop devices with detailed info:

`losetup -a`

- Attach a file to a given loop device:

`sudo losetup /dev/{{loop}} /{{path/to/file}}`

- Attach a file to a new free loop device and scan the device for partitions:

`sudo losetup --show --partscan -f /{{path/to/file}}`

- Attach a file to a read-only loop device:

`sudo losetup --read-only /dev/{{loop}} /{{path/to/file}}`

- Detach all loop devices:

`sudo losetup -D`

- Detach a given loop device:

`sudo losetup -d /dev/{{loop}}`
