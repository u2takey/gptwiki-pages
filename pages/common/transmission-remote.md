# transmission-remote 
## chatgpt 
transmission-remote is a command-line interface for managing the Transmission BitTorrent client. It allows remote control of the Transmission client, which means that you can control the client from another machine over a network.

The basic syntax of the command is as follows:

```
transmission-remote [options] [url]
```

Here, `[options]` are command-line options that can be used with the `transmission-remote` command, and `[url]` is the URL of the Transmission client.

Some of the commonly used options are:

- `-n`: Connect to a remote Transmission client using authentication.
- `-a`: Add a torrent file or magnet link to the Transmission client.
- `-u`: Set the username for authentication.
- `-p`: Set the password for authentication.
- `-S`: Show the status of the current torrents.
- `-l`: List all the torrents in the Transmission client.
- `-t`: Specify a torrent ID to perform an action on a specific torrent.

For example, to add a torrent file to the Transmission client, the command would be:

```
transmission-remote -n 'user:password' -a /path/to/torrent/file.torrent
```

This command connects to a remote Transmission client using the username `user` and the password `password`, and adds the torrent file located at `/path/to/torrent/file.torrent` to the Transmission client.

Similarly, to list all the torrents in the Transmission client, the command would be:

```
transmission-remote -n 'user:password' -l
```

This command connects to a remote Transmission client using the username `user` and the password `password`, and lists all the torrents in the Transmission client. 

## tldr 
 
> Remote control utility for transmission-daemon and transmission.
> More information: <https://transmissionbt.com>.

- Add a torrent file or magnet link to Transmission and download to a specified directory:

`transmission-remote {{hostname}} -a {{torrent|url}} -w {{/path/to/download_directory}}`

- Change the default download directory:

`transmission-remote {{hostname}} -w {{/path/to/download_directory}}`

- List all torrents:

`transmission-remote {{hostname}} --list`

- Start torrent 1 and 2, stop torrent 3:

`transmission-remote {{hostname}} -t "{{1,2}}" --start -t {{3}} --stop`

- Remove torrent 1 and 2, and also delete local data for torrent 2:

`transmission-remote {{hostname}} -t {{1}} --remove -t {{2}} --remove-and-delete`

- Stop all torrents:

`transmission-remote {{hostname}} -t {{all}} --stop`

- Move torrents 1-10 and 15-20 to a new directory (which will be created if it does not exist):

`transmission-remote {{hostname}} -t "{{1-10,15-20}}" --move {{/path/to/new_directory}}`
