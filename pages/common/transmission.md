# transmission 
## chatgpt 
Transmission is a command-line BitTorrent client that allows downloading and uploading of files on the BitTorrent protocol. It is a lightweight and fast client, capable of handling multiple downloads simultaneously. Transmission can be used on different platforms including Linux, macOS, Windows, and FreeBSD.

To use the transmission command, you need to first install the client on your system. Once installed, you can run the command to start the client and begin downloading or uploading files. The basic syntax for the transmission command is as follows:

transmission [options] [arguments]

Here are some of the commonly used options and arguments for the transmission command:

- -h: Displays a help message that lists all available options and their usages.

- -d/--download-dir: Specifies the directory to save downloaded files.

- -u/--upload-limit: Sets the maximum upload speed in Kilobits per second (Kbps).

- -a/--add: Adds the torrent file or magnet link to the download queue.

- -r/--remove: Removes the torrent and associated files from the download queue.

- -s/--stop: Stops downloading or uploading a torrent.

- -l/--list: Displays a list of all active torrents.

- -p/--port: Specifies the listening port for incoming connections.

- -b/--blocklist: Enables and sets an IP blocklist to block connections from certain IP addresses.

The transmission command can be customized further using various configuration options that can be modified through the settings.json file. Overall, the transmission command is a powerful tool for downloading and uploading files using the BitTorrent protocol. 

## tldr 
 
> Transmission is a simple torrent client.
> Transmission isn't a command, but a set of commands. See the pages below.
> More information: <https://transmissionbt.com/>.

- Show the tldr page for running Transmission's daemon:

`tldr transmission-daemon`

- Show the tldr page for interacting with the daemon:

`tldr transmission-remote`

- Show the tldr page for creating torrent files:

`tldr transmission-create`

- Show the tldr page for modifying torrent files:

`tldr transmission-edit`

- Show the tldr page for getting info about torrent files:

`tldr transmission-show`

- Show the tldr page for the deprecated method for interacting with the daemon:

`tldr transmission-cli`
