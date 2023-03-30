# transmission-cli 
## chatgpt 
transmission-cli is a command-line interface (CLI) for the Transmission BitTorrent client. The transmission-cli command is used to interact with the Transmission daemon (transmission-daemon) that runs in the background.

The transmission-cli command is used to perform various tasks such as adding or removing torrents, controlling download/upload speed, setting download priority, configuring encryption, viewing statistics, etc.

Here are some of the common transmission-cli commands:

- transmission-cli -f [torrent_file_path] : Use this command to add a torrent file to Transmission and start downloading it.
- transmission-cli -t [torrent_id] -r : Use this command to delete a torrent from Transmission along with its downloaded files.
- transmission-cli -t [torrent_id] -u [upload_speed] : Use this command to set the upload speed limit for a specific torrent.
- transmission-cli -t [torrent_id] -D : Use this command to set the download priority for a specific torrent to high.
- transmission-cli -t [torrent_id] -s : Use this command to pause or resume a download.

In addition to the above commands, there are many other options available in transmission-cli that can be found by using the "transmission-cli --help" command. Overall, transmission-cli provides a powerful and flexible way to manage torrent downloads through the command line. 

## tldr 
 
> A lightweight, command-line BitTorrent client.
> This tool has been deprecated, please see `transmission-remote`.
> More information: <https://transmissionbt.com>.

- Download a specific torrent:

`transmission-cli {{url|magnet|path/to/file}}`

- Download a torrent to a specific directory:

`transmission-cli --download-dir {{path/to/download_directory}} {{url|magnet|path/to/file}}`

- Create a torrent file from a specific file or directory:

`transmission-cli --new {{path/to/source_file_or_directory}}`

- Set the download speed limit to 50 KB/s:

`transmission-cli --downlimit {{50}} {{url|magnet|path/to/file}}`

- Set the upload speed limit to 50 KB/s:

`transmission-cli --uplimit {{50}} {{url|magnet|path/to/file}}`

- Use a specific port for connections:

`transmission-cli --port {{port_number}} {{url|magnet|path/to/file}}`

- Force encryption for peer connections:

`transmission-cli --encryption-required {{url|magnet|path/to/file}}`

- Use a Bluetack-formatted peer blocklist:

`transmission-cli --blocklist {{blocklist_url|path/to/blocklist}} {{url|magnet|path/to/file}}`
