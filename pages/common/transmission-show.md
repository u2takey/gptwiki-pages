# transmission-show 
## chatgpt 
`transmission-show` is a command used in the Transmission BitTorrent client to display information about a torrent file. It is used to extract information about the torrent, such as its name, size, trackers, files, and pieces.

Here is a breakdown of the different aspects of the command:

-  `transmission-show`: This is the command itself. It is used to display the information about the torrent file.

-  `<filename.torrent>`: This is the name of the torrent file you want to get information about. You need to replace `filename.torrent` with the actual file name.

When you run this command, Transmission will display detailed information about the torrent file in a structured format. The output generally includes:

-  Name of the torrent

-  Size of the torrent

-  Number of files in the torrent

-  Trackers that the torrent is associated with

-  Hashes of the torrent

-  Information about the pieces of the torrent

-  Information about the torrent's metadata

-  Information about the torrent's creation date

This information can be useful for troubleshooting issues with the torrent, and for ensuring that the torrent is legit and safe to download. Overall, the `transmission-show` command is a useful tool for anyone using the Transmission BitTorrent client. 

## tldr 
 
> Get information about a torrent file.
> See also: `transmission`.
> More information: <https://manned.org/transmission-show>.

- Display metadata for a specific torrent:

`transmission-show {{path/to/file.torrent}}`

- Generate a magnet link for a specific torrent:

`transmission-show --magnet {{path/to/file.torrent}}`

- Query a torrent's trackers and print the current number of peers:

`transmission-show --scrape {{path/to/file.torrent}}`
