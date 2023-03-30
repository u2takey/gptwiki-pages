# streamlink 
## chatgpt 
Streamlink is a command-line utility that allows users to watch online video streams in their preferred media player. It can be used to stream live events, sports matches, TV shows, movies, and more.

The basic syntax of the “streamlink” command is as follows:

streamlink [OPTIONS] [URL] [QUALITY]

Here, OPTIONS are the various options that can be passed with the streamlink command. URL is the address of the online video stream that the user wants to watch, and QUALITY is the video quality that the user wants to play the stream in.

Some of the popular options that can be used with the streamlink command are:

--player: This option specifies the name of the media player that the user wants to use to play the stream. By default, Streamlink uses VLC media player, but the user can specify a different player using this option.

--output: This option specifies the output filename where the stream will be saved. The file can be saved in a range of formats including FLV, MP4 or MPEG-TS

--logfile: This option specifies the name of the log file in which all the log information will be registered.

--no-version-check: This option will helps disabling the streamlink version check.

Overall, streamlink is a powerful command-line utility for streaming online videos, and it can be highly customizable using various options available.  It provides a more reliable and stable viewing experience than some of the in-browser streaming services available today.  

## tldr 
 
> Extracts streams from various services and pipes them into a video player of choice.
> More information: <https://streamlink.github.io>.

- Attempt to extract streams from the URL specified, and if it's successful, print out a list of available streams to choose from:

`streamlink {{example.com/stream}}`

- Open a stream with the specified quality:

`streamlink {{example.com/stream}} {{720p60}}`

- Select the highest or lowest available quality:

`streamlink {{example.com/stream}} {{best|worst}}`

- Specify which player to use to feed stream data to (VLC is used by default if found):

`streamlink --player={{mpv}} {{example.com/stream}} {{best}}`

- Specify the amount of time to skip from the beginning of the stream. For live streams, this is a negative offset from the end of the stream (rewind):

`streamlink --hls-start-offset {{[HH:]MM:SS}} {{example.com/stream}} {{best}}`

- Skip to the beginning of a live stream, or as far back as possible:

`streamlink --hls-live-restart {{example.com/stream}} {{best}}`

- Write stream data to a file instead of playing it:

`streamlink --output {{path/to/file.ts}} {{example.com/stream}} {{best}}`

- Open the stream in the player, while at the same time writing it to a file:

`streamlink --record {{path/to/file.ts}} {{example.com/stream}} {{best}}`
