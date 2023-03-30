# ffmpeg 
## chatgpt 
FFmpeg is a free and open-source command-line tool that can decode, encode, and transcode video and audio files. It supports a wide range of codecs, containers, and protocols, and can handle various video and audio formats, resolutions, and frame rates. FFmpeg can also perform basic video and audio editing tasks, such as cutting, merging, and adding subtitles, and can process multiple files in batch mode. Some examples of FFmpeg commands include:

- `ffmpeg -i input.mp4 output.avi`: This command converts a MP4 video file named "input.mp4" into an AVI file named "output.avi".
- `ffmpeg -i input.wav -acodec libmp3lame -ab 128k output.mp3`: This command converts a WAV audio file named "input.wav" into an MP3 file named "output.mp3" using the LAME encoder at a bitrate of 128 kbps.
- `ffmpeg -i input.mp4 -c:v copy -c:a aac -strict experimental output.mp4`: This command copies the video stream of a MP4 file named "input.mp4" without transcoding it, and transcodes the audio stream into AAC format with the experimental AAC encoder. The output file is named "output.mp4".
- `ffmpeg -i input.mp4 -ss 00:01:00 -t 00:00:30 -c copy output.mp4`: This command extracts a 30-second clip from a MP4 file named "input.mp4" starting at the 1-minute mark, without transcoding it, and saves it as a new file named "output.mp4".
- `ffmpeg -i input.mp4 -vf subtitles=subs.srt output.mp4`: This command adds subtitle tracks from a separate SRT file named "subs.srt" to a MP4 video file named "input.mp4", and saves it as a new file named "output.mp4" using the default video codec and audio codec. 

## tldr 
 
> Video conversion tool.
> More information: <https://ffmpeg.org>.

- Extract the sound from a video and save it as MP3:

`ffmpeg -i {{video.mp4}} -vn {{sound}}.mp3`

- Save a video as GIF, scaling the height to 1000px and setting framerate to 15:

`ffmpeg -i {{video.mp4}} -vf 'scale=-1:{{1000}}' -r {{15}} {{output.gif}}`

- Combine numbered images (`frame_1.jpg`, `frame_2.jpg`, etc) into a video or GIF:

`ffmpeg -i {{frame_%d.jpg}} -f image2 {{video.mpg|video.gif}}`

- Quickly extract a single frame from a video at time mm:ss and save it as a 128x128 resolution image:

`ffmpeg -ss {{mm:ss}} -i {{video.mp4}} -frames 1 -s {{128x128}} -f image2 {{image.png}}`

- Trim a video from a given start time mm:ss to an end time mm2:ss2 (omit the -to flag to trim till the end):

`ffmpeg -ss {{mm:ss}} -to {{mm2:ss2}} -i {{video.mp4}} -codec copy {{output.mp4}}`

- Convert AVI video to MP4. AAC Audio @ 128kbit, h264 Video @ CRF 23:

`ffmpeg -i {{input_video}}.avi -codec:a aac -b:a 128k -codec:v libx264 -crf 23 {{output_video}}.mp4`

- Remux MKV video to MP4 without re-encoding audio or video streams:

`ffmpeg -i {{input_video}}.mkv -codec copy {{output_video}}.mp4`

- Convert MP4 video to VP9 codec. For the best quality, use a CRF value (recommended range 15-35) and -b:v MUST be 0:

`ffmpeg -i {{input_video}}.mp4 -codec:v libvpx-vp9 -crf {{30}} -b:v 0 -codec:a libopus -vbr on -threads {{number_of_threads}} {{output_video}}.webm`
