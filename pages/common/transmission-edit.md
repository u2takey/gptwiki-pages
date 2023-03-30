# transmission-edit 
## chatgpt 
The `transmission-edit` command is a command-line tool used to modify or edit the settings and options of a BitTorrent client known as Transmission. It allows a user to configure advanced settings, add or remove torrents, change the download priority, and modify the bandwidth allocation of torrents.

The syntax of the command is:

```
transmission-edit [options] torrent-file
```

The `options` parameter consists of various command-line switches that modify the behavior of the `transmission-edit` command. Some of the commonly used options include:

- `-a <file>`: Adds a torrent to the Transmission client.
- `-r`: Removes a torrent from the Transmission client.
- `-p <priority>`: Sets the download priority of a torrent. The priority can be either `high`, `normal`, `low`, or `no` (which means that the torrent will be paused).
- `-u <integer>`: Sets the upload bandwidth limit for Transmission.
- `-d <integer>`: Sets the download bandwidth limit for Transmission.
- `-i <IP address>`: Sets the IP address used for incoming connections.

The `torrent-file` parameter is the path to the torrent file that you want to edit. This file contains all the necessary information for Transmission to download and share the files associated with the torrent.

In summary, the `transmission-edit` command is used to configure and manage the settings of the Transmission BitTorrent client. It provides a variety of options that allow users to modify the behavior of the client and manage the torrents that are being downloaded or uploaded. 

## tldr 
 
> Modify announce URLs from torrent files.
> See also: `transmission`.
> More information: <https://manned.org/transmission-edit>.

- Add or remove a URL from a torrent's announce list:

`transmission-edit --{{add|delete}} {{http://example.com}} {{path/to/file.torrent}}`

- Update a tracker's passcode in a torrent file:

`transmission-edit --replace {{old-passcode}} {{new-passcode}} {{path/to/file.torrent}}`
