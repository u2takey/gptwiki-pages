# mediainfo 
## chatgpt 
Mediainfo is a command-line program that displays technical information about audio and video files. 

When the command `mediainfo` is executed, the program runs and prompts the user to specify a file or multiple files, whose technical details they would like to retrieve. By default, the output includes the following information: 

- File format 
- Codec used for audio and video 
- Bitrate 
- Frame rate 
- Resolution 
- Aspect ratio 
- Duration 
- Container formats and more.

Mediainfo can be useful for troubleshooting audio and video issues, checking compatibility for playback, or simply to learn more about the technical specifications of a media file. 

The `mediainfo` command also has various options that can be used to customize the output or limit the information provided. For example, `-f` can be used to change the output format (e.g., XML or JSON) and `- Language` can be used to specify the language of the output. 

Overall, the `mediainfo` command is a powerful and versatile tool for accessing and analyzing media file information from the command line. 

## tldr 
 
> Display metadata from video and audio files.
> More information: <https://mediaarea.net/MediaInfo>.

- Display metadata for a given file in the console:

`mediainfo {{file}}`

- Store the output to a given file along with displaying in the console:

`mediainfo --Logfile={{out.txt}} {{file}}`

- Display the list of metadata attributes that can be extracted:

`mediainfo --Info-Parameters`
