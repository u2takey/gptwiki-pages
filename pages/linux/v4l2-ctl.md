# v4l2-ctl 
## chatgpt 
The v4l2-ctl command is a tool used to interact with the Video4Linux2 (V4L2) driver, which is the kernel module responsible for the control and management of video devices on Linux operating systems. 

When running the v4l2-ctl command, various options can be specified to manipulate the parameters and settings for a particular video device. Some of the functions that can be performed using v4l2-ctl include:

- Querying the capabilities of a device: The -d option can be used to specify the video device to query, and the --all option can be used to display all the capabilities of the device, including supported video formats, supported resolutions, and control options.

- Modifying control settings: The -c option can be used to specify the control to modify, and the desired value can be specified using the --set-ctrl option. For example, v4l2-ctl -d /dev/video0 -c exposure_auto=3 will set the auto exposure mode to 'Manual Mode'.

- Capturing video and audio: The -i option can be used to specify the input to capture from, and the -P option can be used to specify the pixel format of the captured frames. The captured frames can then be saved to a file by redirecting the output to a file using the '>' operator.

Overall, v4l2-ctl is a powerful tool for controlling and managing video devices on Linux systems, and provides a way to fine-tune and customize the behavior of video-related applications. 

## tldr 
 
> Control video devices.
> More information: <https://manned.org/v4l2-ctl>.

- List all video devices:

`v4l2-ctl --list-devices`

- List supported video formats and resolutions of default video device `/dev/video0`:

`v4l2-ctl --list-formats-ext`

- List supported video formats and resolutions of a specific video device:

`v4l2-ctl --list-formats-ext --device {{path/to/video_device}}`

- Get all details of a video device:

`v4l2-ctl --all --device {{path/to/video_device}}`

- Capture a JPEG photo with a specific resolution from video device:

`v4l2-ctl --device {{path/to/video_device}} --set-fmt-video=width={{width}},height={{height}},pixelformat=MJPG --stream-mmap --stream-to={{path/to/output.jpg}} --stream-count=1`

- Capture a raw video stream from video device:

`v4l2-ctl --device {{path/to/video_device}} --set-fmt-video=width={{width}},height={{height}},pixelformat={{format}} --stream-mmap --stream-to={{path/to/output}} --stream-count={{number_of_frames_to_capture}}`

- List all video device's controls and their values:

`v4l2-ctl --list-ctrls --device {{/path/to/video_device}}`
