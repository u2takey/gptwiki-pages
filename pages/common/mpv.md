# mpv 
## chatgpt 
mpv is a free and open-source media player software for Windows, macOS, Linux, and Android. It supports a wide range of audio and video formats, including network streams, DVD and Blu-ray video discs, and various file containers such as AVI, MP4, MOV, and MKV.

The mpv command is executed in a command-line interface or terminal to launch the mpv media player with the specified file or URL as input. Here's an example:

```
mpv video.mp4
```

This command launches mpv and plays the video.mp4 file. mpv automatically detects the format and codecs of the file and selects the appropriate audio and video tracks, subtitles, and aspect ratio.

mpv has many advanced features and options that can be customized through command line flags, configuration files, and input commands during playback. Some common options include:

- control playback speed with --speed option
- adjust audio/video delay with --audio-delay/--sub-delay options
- change audio track with --audio-file/--audio-lang options
- add subtitles with --sub-file/--sub-lang options
- choose video format with --vo option
- select audio output device with --ao option
- enable hardware acceleration with --hwdec/--vo options

For more information about all the available options, refer to the mpv manual or online documentation. 

## tldr 
 
> A audio/video player based on MPlayer.
> More information: <https://mpv.io>.

- Play a video or audio file:

`mpv {{path/to/file}}`

- Play a video or audio file from a URL:

`mpv '{{https://www.youtube.com/watch?v=dQw4w9WgXcQ}}'`

- Jump backward/forward 5 seconds:

`LEFT <or> RIGHT`

- Jump backward/forward 1 minute:

`DOWN <or> UP`

- Decrease or increase playback speed by 10%:

`[ <or> ]`

- Play a file at a specified speed (0.01 to 100, default 1):

`mpv --speed {{speed}} {{path/to/file}}`

- Play a file using a profile defined in the `mpv.conf` file:

`mpv --profile {{profile_name}} {{path/to/file}}`

- Display the output of webcam or other video input device:

`mpv /dev/{{video0}}`
