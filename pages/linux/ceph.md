# ceph 
## chatgpt 
"Ceph" is a command-line utility used to interact with the Ceph distributed storage system. Ceph is an open-source software-defined storage platform that provides object, block, and file storage using a distributed architecture. 

When the "ceph" command is entered, the utility presents a list of subcommands that can be used to perform various functions related to Ceph storage. Some of the common subcommands include:

- "ceph health": This subcommand returns the current health status of the Ceph cluster. It checks for any problems in the system and provides information about any issues that need attention.

- "ceph mon": This is a subcommand used for managing the Ceph monitor nodes in the cluster. It allows administrators to add or remove monitors, view status information, and perform other monitoring-related tasks.

- "ceph osd": This subcommand is used for managing the Ceph object storage daemons (OSDs) that store data in the system. It allows admins to view the status of OSDs, adjust their settings, and perform other OSD-related tasks.

- "ceph pg": This subcommand is used for managing placement groups (PGs) in the Ceph cluster. PGs are used to distribute data across OSDs and maintain data redundancy. This subcommand allows admins to view PG status, adjust PG settings, and perform other PG-related tasks.

Overall, the "ceph" command is a powerful tool used to manage and maintain the Ceph distributed storage system. Its subcommands provide a wide range of functions that admins can use to ensure that the storage platform is running smoothly and efficiently. 

## tldr 
 
> A unified storage system.
> More information: <https://ceph.io>.

- Check cluster health status:

`ceph status`

- Check cluster usage stats:

`ceph df`

- Get the statistics for the placement groups in a cluster:

`ceph pg dump --format {{plain}}`

- Create a storage pool:

`ceph osd pool create {{pool_name}} {{page_number}}`

- Delete a storage pool:

`ceph osd pool delete {{pool_name}}`

- Rename a storage pool:

`ceph osd pool rename {{current_name}} {{new_name}}`

- Self-repair pool storage:

`ceph pg repair {{pool_name}}`
