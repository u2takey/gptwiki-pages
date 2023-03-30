# mdadm 
## chatgpt 
mdadm is a command-line tool used in Linux to manage and configure software RAID arrays. The term "md" stands for multiple devices, which is suitable for software-based RAID configurations where multiple disks are combined into a single logical unit.

The mdadm command has various options that can be used to create, manage and monitor RAID arrays. Here are some of the commonly used options:

- --create: This option is used to create a new RAID array. It requires parameters such as RAID level, device names, and other configuration options.

- --assemble: This option is used to assemble an existing RAID array. It is used when a system is rebooted or when a disk is replaced.

- --detail: This option provides detailed information about the RAID arrays currently configured, including their status, devices used, RAID level, etc.

- --manage: This option allows you to manage an existing RAID array. It provides various options to add or remove devices, set the layout, or change the RAID level.

- --fail: This option is used to mark a device as failed in the RAID array. When a device fails, the data is automatically rebuilt on the remaining devices.

Overall, the mdadm command is a powerful tool that allows you to create, manage, and monitor RAID arrays for improved data reliability and availability. 

## tldr 
 
> RAID management utility.
> More information: <https://manned.org/mdadm>.

- Create array:

`sudo mdadm --create {{/dev/md/MyRAID}} --level {{raid_level}} --raid-devices {{number_of_disks}} {{/dev/sdXN}}`

- Stop array:

`sudo mdadm --stop {{/dev/md0}}`

- Mark disk as failed:

`sudo mdadm --fail {{/dev/md0}} {{/dev/sdXN}}`

- Remove disk:

`sudo mdadm --remove {{/dev/md0}} {{/dev/sdXN}}`

- Add disk to array:

`sudo mdadm --assemble {{/dev/md0}} {{/dev/sdXN}}`

- Show RAID info:

`sudo mdadm --detail {{/dev/md0}}`

- Reset disk by deleting RAID metadata:

`sudo mdadm --zero-superblock {{/dev/sdXN}}`
