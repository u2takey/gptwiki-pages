# fatlabel 
## chatgpt 
`fatlabel` is a command used to set or view the label, which is essentially the name of a FAT (File Allocation Table) file system volume.

To view the label of a FAT file system volume, the following command can be used:

```
fatlabel [device]
```

Here, `[device]` specifies the device file or partition of the FAT file system volume. For example, if the device file for the volume is `/dev/sdb1`, the command would be:

```
fatlabel /dev/sdb1
```

The command will output the current label of the volume.

To set or change the label of a FAT file system volume, the following command can be used:

```
fatlabel [device] [label]
```

Here, `[device]` specifies the device file or partition of the FAT file system volume, and `[label]` specifies the new label to be set. For example, to set the label of `/dev/sdb1` to "MY_VOLUME", the command would be:

```
fatlabel /dev/sdb1 MY_VOLUME
```

Note that the label can only be up to 11 characters long and can contain letters, numbers, underscores, and hyphens. Additionally, the label is case-insensitive and cannot contain spaces or other special characters. 

## tldr 
 
> Sets or gets the label of a FAT32 partition.
> More information: <https://manned.org/fatlabel>.

- Get the label of a FAT32 partition:

`fatlabel {{/dev/sda1}}`

- Set the label of a FAT32 partition:

`fatlabel {{/dev/sdc3}} "{{new_label}}"`
