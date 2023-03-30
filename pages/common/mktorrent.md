# mktorrent 
## chatgpt 
mktorrent is a command-line tool used to create BitTorrent metafiles, also known as .torrent files. These files contain information about the files being shared, and the tracker(s) that are hosting the torrent.

To use mktorrent, you first need to have the files you want to share in a folder on your computer. Then, you would run the mktorrent command with the appropriate parameters.

Here is an example command:

`mktorrent -a "http://tracker.example.com/announce" -o test.torrent my_files_folder/`

Let's break down this command:

- `mktorrent` is the name of the command.
- `-a "http://tracker.example.com/announce"` specifies the tracker that will be used to host the torrent. You can use one or multiple trackers, separated by commas. This parameter is optional, but recommended, as it helps users find and connect to your torrent.
- `-o test.torrent` specifies the name of the .torrent file that will be created. You can choose any name you like, but it should have the extension .torrent.
- `my_files_folder/` is the path to the folder that contains the files you want to share. Make sure to include the trailing slash.

Once you run the command, mktorrent will create a .torrent file in the current directory. You can then share this file with others, either by uploading it to a website or sending it directly to other users. When someone downloads and opens the .torrent file, their BitTorrent client will use the tracker information to find peers who are sharing the same files, and download them from those peers. 

## tldr 
 
> A CLI utility to create BitTorrent metainfo files.
> More information: <https://github.com/Rudde/mktorrent>.

- Create a torrent with 2^21 KB as the piece size:

`mktorrent -a {{tracker_announce_url}} -l {{21}} -o {{path/to/example.torrent}} {{path/to/file_or_directory}}`

- Create a private torrent with a 2^21 KB piece size:

`mktorrent -p -a {{tracker_announce_url}} -l {{21}} -o {{path/to/example.torrent}} {{path/to/file_or_directory}}`

- Create a torrent with a comment:

`mktorrent -c "{{comment}}" -a {{tracker_announce_url}} -l {{21}} -o {{path/to/example.torrent}} {{path/to/file_or_directory}}`

- Create a torrent with multiple trackers:

`mktorrent -a {{tracker_announce_url,tracker_announce_url_2}} -l {{21}} -o {{path/to/example.torrent}} {{path/to/file_or_directory}}`

- Create a torrent with web seed URLs:

`mktorrent -a {{tracker_announce_url}} -w {{web_seed_url}} -l {{21}} -o {{path/to/example.torrent}} {{path/to/file_or_directory}}`
