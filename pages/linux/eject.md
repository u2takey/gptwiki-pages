# eject 
## chatgpt 
The `eject` command is a Linux and Unix-based utility used to eject removable storage devices such as CD-ROMs, DVDs, and external hard drives. 

When you enter the command `eject` into your terminal, it will automatically eject the mounted CD-ROM, DVD, or other removable device from your system. You can also use the command along with a specific device name or path to eject only that particular device. 

For example, to eject a CD-ROM with the device name "/dev/cdrom", you would enter the following command:

```
eject /dev/cdrom
```

The `eject` command can also be used to lock the tray of an optical drive or to toggle the power state of a SATA connection. These options require additional flags to be used with the command. 

Overall, the `eject` command is a simple and useful tool for quickly and easily ejecting removable storage devices from your Linux or Unix-based system. 

## tldr 
 
> Eject cds, floppy disks and tape drives.
> More information: <https://manned.org/eject>.

- Display the default device:

`eject -d`

- Eject the default device:

`eject`

- Eject a specific device (the default order is cd-rom, scsi, floppy and tape):

`eject {{/dev/cdrom}}`

- Toggle whether a device's tray is open or closed:

`eject -T {{/dev/cdrom}}`

- Eject a cd drive:

`eject -r {{/dev/cdrom}}`

- Eject a floppy drive:

`eject -f {{/mnt/floppy}}`

- Eject a tape drive:

`eject -q {{/mnt/tape}}`
