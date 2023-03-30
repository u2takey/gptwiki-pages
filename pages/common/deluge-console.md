# deluge-console 
## chatgpt 
deluge-console is a command-line interface (CLI) tool for managing a Deluge BitTorrent client installation. The Deluge BitTorrent client is a free and open-source software that allows users to download and share files using the BitTorrent protocol.

The deluge-console command is used to access and manage the Deluge client from the terminal. Once the command is run, the user will be presented with an interactive shell prompt where commands can be entered to interact with the Deluge client.

Some of the common tasks that can be performed using the deluge-console include adding or removing torrent files, setting upload and download speed limits, managing torrents, and setting preferences.

Here are some examples of how to use the deluge-console command:

- To start the console, simply run the following command:

  ```
  deluge-console
  ```

  This will open the interactive shell prompt where you can enter commands.

- To add a torrent file, you can use the "add" command followed by the path to the torrent file. For example:

  ```
  add /path/to/my/torrent/file.torrent
  ```

- To list all active torrents, use the "info" command:

  ```
  info
  ```

- To set a download speed limit, use the "config" command followed by the maximum download speed in bytes per second (B/s). For example:

  ```
  config --set max_download_speed 50000
  ```

  This would set the maximum download speed to 50 kB/s.

- To exit the console, simply use the "exit" command:

  ```
  exit
  ```

  This will close the interactive shell and return you to the command prompt. 

## tldr 
 
> An interactive interface for the Deluge BitTorrent client.
> More information: <https://deluge-torrent.org>.

- Start the interactive console interface:

`deluge-console`

- Connect to a Deluge daemon instance:

`connect {{hostname}}:{{port}}`

- Add a torrent to the daemon:

`add {{url|magnet|path/to/file}}`

- Display information about all torrents:

`info`

- Display information about a specific torrent:

`info {{torrent_id}}`

- Pause a torrent:

`pause {{torrent_id}}`

- Resume a torrent:

`resume {{torrent_id}}`

- Remove a torrent from the daemon:

`rm {{torrent_id}}`
