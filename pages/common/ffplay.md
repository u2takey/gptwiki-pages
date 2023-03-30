# ffplay 
## chatgpt 
ffplay is a command-line tool used for playing multimedia files. It is a part of the FFmpeg project which is a widely used, open-source multimedia framework that includes tools for recording, streaming, and converting audio and video files. 

When executed, the ffplay command starts a media player that can play a wide range of audio and video formats. The player is designed to be used from the command line, and it provides a number of options for controlling the playback, such as adjusting the volume, seeking to a specific time in the media, and changing the playback speed. 

Some popular input formats it supports include MP4, MOV, AVI, MPEG, and many others. The ffplay command can also be used for testing audio and video streams by specifying the URL of the stream as the input source. In this case, it can also be used to validate streaming parameters, such as bitrates and stream protocols.

In summary, the ffplay command is a powerful tool for playing audio and video files, and testing audio and video streams, as well as testing audio and video codecs and other metadata information. 

## tldr 
 
> A simple and portable media player using the FFmpeg libraries and the SDL library.
> More information: <https://ffmpeg.org/ffplay-all.html>.

- Play a media file:

`ffplay {{path/to/file}}`

- Play a video and show motion vectors in real time:

`ffplay -flags2 +export_mvs -vf codecview=mv=pf+bf+bb {{path/to/file}}`

- Show only video keyframes:

`ffplay -vf select="{{eq(pict_type\,PICT_TYPE_I)}}" {{path/to/file}}`
