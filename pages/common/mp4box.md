# mp4box 
## chatgpt 
MP4Box is a multimedia tool used to manipulate MP4 files. It is a command line tool that can be used to create, edit, and analyze MP4 files. Some common commands used with MP4Box include:

1. -add: This command is used to add a media file to an existing MP4 file. For example, "MP4Box -add input.avi output.mp4" will add the AVI file "input.avi" to the MP4 file "output.mp4".

2. -split: This command is used to split a large MP4 file into smaller segments. For example, "MP4Box -split 1000 output.mp4" will split the file "output.mp4" into 1000MB segments.

3. -dash: This command is used to create a DASH (Dynamic Adaptive Streaming over HTTP) manifest file. For example, "MP4Box -dash 1000 -segment-name output_ output.mp4" will create a DASH manifest and segment files with a segment duration of 1000ms and a segment name prefix of "output_".

4. -info: This command is used to display information about an MP4 file. For example, "MP4Box -info output.mp4" will display information about the file "output.mp4", such as the video and audio codecs used, the duration, and the bitrates.

5. -extract: This command is used to extract a specific track or set of tracks from an MP4 file. For example, "MP4Box -extract 1 output.mp4" will extract the first track from the file "output.mp4".

Overall, MP4Box is a powerful tool for working with MP4 files and can be used for a variety of tasks, including editing, conversion, and streaming. 

## tldr 
 
> MPEG-4 Systems Toolbox - Muxes streams into MP4 container.
> More information: <https://gpac.wp.imt.fr/mp4box>.

- Display information about an existing MP4 file:

`mp4box -info {{path/to/file}}`

- Add an SRT subtitle file into an MP4 file:

`mp4box -add {{input_subs.srt}}:lang=eng -add {{input.mp4}} {{output.mp4}}`

- Combine audio from one file and video from another:

`mp4box -add {{input1.mp4}}#audio -add {{input2.mp4}}#video {{output.mp4}}`
