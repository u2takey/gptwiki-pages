# zramctl 
## chatgpt 
The `zramctl` command is used to control and display the status of zram devices in Linux. Zram is a kernel module that provides a compressed block device in RAM. It can be used as a swap device or for storing temporary files.

The `zramctl` command can be used with various options to perform different actions. Here are some common options:

- `-h` or `--help`: displays the help message for `zramctl`.
- `-f` or `--find`: finds an unused zram device and initializes it.
- `-a` or `--add`: adds a new zram device with a specified size.
- `-r` or `--reset`: resets the compression statistics for a zram device.
- `-s` or `--size`: sets the size of a zram device.
- `-t` or `--target`: sets the compression algorithm used by a zram device.

When executed without any options, `zramctl` displays a summary of all the zram devices currently in use, including their ID, size, compression algorithm, and compression ratio.

Overall, `zramctl` is a useful tool for managing zram devices in Linux systems. 

## tldr 
 
> Setup and control zram devices.
> Use `mkfs` or `mkswap` to format zram devices to partitions.
> More information: <https://manned.org/zramctl>.

- Check if zram is enabled:

`lsmod | grep -i zram`

- Enable zram with a dynamic number of devices (use `zramctl` to configure devices further):

`sudo modprobe zram`

- Enable zram with exactly 2 devices:

`sudo modprobe zram num_devices={{2}}`

- Find and initialize the next free zram device to a 2 GB virtual drive using LZ4 compression:

`sudo zramctl --find --size {{2GB}} --algorithm {{lz4}}`

- List currently initialized devices:

`zramctl`
