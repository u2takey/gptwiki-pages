# handbrakecli 
## chatgpt 
HandbrakeCLI is a command-line interface for the Handbrake video transcoding software. HandbrakeCLI allows users to convert video files from one format to another, adjust video settings such as resolution and bit rate, and apply filters to enhance the quality of the video.

To use HandbrakeCLI, users must first download and install the Handbrake software onto their computer. Once installed, users can open a command prompt or terminal window and enter the command "HandbrakeCLI" followed by various options and parameters to specify the desired video conversion settings.

Some common parameters that can be used with HandbrakeCLI include:

- "-i" to specify the input video file
- "-o" to specify the output file location and name
- "--preset" to choose a pre-configured transcoding preset
- "--encoder" to choose the video encoder to use
- "--vb" to set the video bitrate
- "--s" to set the output video resolution
- "--crop" to crop the video

Users can also specify additional custom filters and settings using specific HandbrakeCLI commands and syntax.

Overall, HandbrakeCLI is a powerful tool for video transcoding and customization, requiring some technical knowledge and command-line proficiency to use effectively. 

## tldr 
 
> Command-line interface to the HandBrake video conversion and DVD ripping tool.
> More information: <https://handbrake.fr/>.

- Convert a video file to MKV (AAC 160kbit audio and x264 CRF20 video):

`handbrakecli --input {{input.avi}} --output {{output.mkv}} --encoder x264 --quality 20 --ab 160`

- Resize a video file to 320x240:

`handbrakecli --input {{input.mp4}} --output {{output.mp4}} --width 320 --height 240`

- List available presets:

`handbrakecli --preset-list`

- Convert an AVI video to MP4 using the Android preset:

`handbrakecli --preset="Android" --input {{input.ext}} --output {{output.mp4}}`

- Print the content of a DVD, getting the CSS keys in the process:

`handbrakecli --input {{/dev/sr0}} --title 0`

- Rip the first track of a DVD in the specified device. Audiotracks and subtitle languages are specified as lists:

`handbrakecli --input {{/dev/sr0}} --title 1 --output {{out.mkv}} --format av_mkv --encoder x264 --subtitle {{1,4,5}} --audio {{1,2}} --aencoder copy --quality {{23}}`
