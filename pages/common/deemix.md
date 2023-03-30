# deemix 
## chatgpt 
Deemix is a command-line tool used for downloading and managing music from Deezer. It allows users to download songs, playlists, and albums in various qualities and formats, including MP3, FLAC, AAC, and OGG. Deemix can also automatically tag and organize the downloaded music.

To use Deemix, the user needs to open the terminal and enter the command "deemix" followed by the required parameters. For example, "deemix -p" opens the web interface of Deemix and "deemix -u [username] -p [password] [link]" downloads the music from the link provided with the user's Deezer account credentials.

Overall, Deemix is a powerful tool for music enthusiasts who want to download and manage their favorite tracks from Deezer. However, it requires some technical knowledge to use as it is a command-line tool. 

## tldr 
 
> A barebone deezer downloader library built from the ashes of Deezloader Remix.
> It can be used as a standalone CLI app or implemented in a UI using the API.
> More information: <https://deemix.app>.

- Download a track or playlist:

`deemix {{https://www.deezer.com/us/track/00000000}}`

- Download track / playlist at a specific bitrate:

`deemix --bitrate {{FLAC|MP3}} {{url}}`

- Download to a specific path:

`deemix --bitrate {{bitrate}} --path {{path}} {{url}}`

- Create a portable deemix config in the current directory:

`deemix --portable --bitrate {{bitrate}} --path {{path}} {{url}}`
