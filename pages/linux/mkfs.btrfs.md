# mkfs.btrfs 
## chatgpt 
The `mkfs.btrfs` command is a Linux command used to create a new Btrfs (B-tree file system) filesystem on a disk or logical volume. 

Here's a breakdown of the command:

`mkfs` is a command that stands for "make filesystem". It is used to create a new filesystem on a storage device.

`.btrfs` is the specific file system type. This indicates that the command is creating a Btrfs filesystem.

When the `mkfs.btrfs` command is executed, it will create a new Btrfs filesystem on the specified device. This command can be used with a number of options to customize the file system creation process, such as setting the block size, selecting RAID level, or specifying a label for the filesystem.

Overall, `mkfs.btrfs` is a critical command for Linux users who want to make use of the robustness and advanced features of Btrfs filesystems. 

## tldr 
 
> Create a btrfs filesystem.
> Defaults to `raid1`, which specifies 2 copies of a given data block spread across 2 different devices.
> More information: <https://btrfs.readthedocs.io/en/latest/mkfs.btrfs.html>.

- Create a btrfs filesystem on a single device:

`sudo mkfs.btrfs --metadata single --data single {{/dev/sda}}`

- Create a btrfs filesystem on multiple devices with raid1:

`sudo mkfs.btrfs --metadata raid1 --data raid1 {{/dev/sda}} {{/dev/sdb}} {{/dev/sdN}}`

- Set a label for the filesystem:

`sudo mkfs.btrfs --label "{{label}}" {{/dev/sda}} [{{/dev/sdN}}]`
