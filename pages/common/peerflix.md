# peerflix 
## chatgpt 
Peerflix is a command-line tool used for streaming torrents. It allows users to stream videos from torrent files without downloading the entire file. The command "peerflix" launches the tool and specifies the torrent file to be streamed, as well as any optional arguments.

The basic syntax of the command is as follows:

peerflix [torrent-file] [options]

Here, [torrent-file] is the path or URL to the torrent file that you want to stream, and [options] are any additional parameters you want to pass.

Some common options for peerflix command include:

- -p or --port: Specify the port number to listen for incoming connections. For example, "peerflix file.torrent --port 3000" will use port number 3000.
- -q or --quiet: Suppress the console output, which is useful for running the tool in the background.
- -m or --magnet: Use this option if the [torrent-file] is a magnet link instead of a .torrent file.
- -v or --vlc: Specify the path to the VLC player executable file. This option is used to play the stream in a different media player than the default one.

Once the peerflix command is executed with the necessary options, it will start streaming the video specified in the torrent file. It will also listen for incoming connections from other peers who have the same file, enabling faster streaming speeds. As the video is streamed, it will be cached on the local disk and can be played back from there afterwards. 

## tldr 
 
> Stream video- or audio-based torrents to a media player.
> More information: <https://github.com/mafintosh/peerflix>.

- Stream the largest media file in a torrent:

`peerflix "{{torrent_url|magnet_link}}"`

- List all streamable files contained in a torrent (given as a magnet link):

`peerflix "{{magnet:?xt=urn:btih:0123456789abcdef0123456789abcdef01234567}}" --list`

- Stream the largest file in a torrent, given as a torrent URL, to VLC:

`peerflix "{{http://example.net/music.torrent}}" --vlc`

- Stream the largest file in a torrent to MPlayer, with subtitles:

`peerflix "{{torrent_url|magnet_link}}" --mplayer --subtitles {{subtitle-file.srt}}`

- Stream all files from a torrent to Airplay:

`peerflix "{{torrent_url|magnet_link}}" --all --airplay`
