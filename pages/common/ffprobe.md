# ffprobe 
## chatgpt 
ffprobe is a command-line tool that is used to analyze audio and video files. It is a part of the FFmpeg multimedia framework, which is a collection of libraries and executables that perform audio and video processing.

When you run the ffprobe command followed by the name of an audio or video file, it provides detailed information about that particular file. This information includes the file format, duration, encoding, bit rate, and many other technical details.

For example, if you run the following command:

```
ffprobe myvideo.mp4
```

The output might include information about the video resolution, frames per second, and audio bit rate.

The ffprobe command can be useful for troubleshooting issues with audio and video playback, and for ensuring that your media files are in the correct format and have the necessary technical specifications for their intended use. 

## tldr 
 
> Multimedia stream analyzer.
> More information: <https://ffmpeg.org/ffprobe.html>.

- Display all available stream info for a media file:

`ffprobe -v error -show_entries {{input.mp4}}`

- Display media duration:

`ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 {{input.mp4}}`

- Display the frame rate of a video:

`ffprobe -v error -select_streams v:0 -show_entries stream=avg_frame_rate -of default=noprint_wrappers=1:nokey=1 {{input.mp4}}`

- Display the width or height of a video:

`ffprobe -v error -select_streams v:0 -show_entries stream={{width|height}} -of default=noprint_wrappers=1:nokey=1 {{input.mp4}}`

- Display the average bit rate of a video:

`ffprobe -v error -select_streams v:0 -show_entries stream=bit_rate -of default=noprint_wrappers=1:nokey=1 {{input.mp4}}`
