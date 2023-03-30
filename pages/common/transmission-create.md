# transmission-create 
## chatgpt 
transmission-create is a command used in the Transmission BitTorrent client to create a new torrent file.

The syntax for the command is as follows:

transmission-create [OPTIONS] [FILE(S) OR DIRECTORY]

Here are the main options for transmission-create:

-d, --tracker URL : specify the tracker URL for the torrent
-o, --outfile FILE : specify the name of the .torrent file to be created
-p, --private : mark the torrent as private
-s, --src TRACKER_URL : specify the source tracker URL

To create a new torrent file using transmission-create, you need to provide the path to the file or directory you want to create a torrent of in the command line. The command will then calculate the hash values for each file in the directory and create a new .torrent file that can be shared with others.

For example, to create a torrent of a directory called "Music" and save the resulting .torrent file as "music.torrent", you would run the following command:

transmission-create -o music.torrent Music

This command would create a new .torrent file called "music.torrent" in the current directory that includes all the files in the "Music" directory. 

## tldr 
 
> A CLI utility to create BitTorrent .torrent files.
> More information: <https://manned.org/transmission-create>.

- Create a torrent with 2048 KB as the piece size:

`transmission-create -o {{path/to/example.torrent}} --tracker {{tracker_announce_url}} --piecesize {{2048}} {{path/to/file_or_directory}}`

- Create a private torrent with a 2048 KB piece size:

`transmission-create -p -o {{path/to/example.torrent}} --tracker {{tracker_announce_url}} --piecesize {{2048}} {{path/to/file_or_directory}}`

- Create a torrent with a comment:

`transmission-create -o {{path/to/example.torrent}} --tracker {{tracker_url1}} -c {{comment}} {{path/to/file_or_directory}}`

- Create a torrent with multiple trackers:

`transmission-create -o {{path/to/example.torrent}} --tracker {{tracker_url1}} --tracker {{tracker_url2}} {{path/to/file_or_directory}}`

- Show help page:

`transmission-create --help`
