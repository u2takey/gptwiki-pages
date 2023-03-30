# you-get 
## chatgpt 
"You-get" is a command line utility tool used to download videos and images from various websites. It's an open-source media downloader tool capable of running on Windows, Linux/Unix, and macOS. This command helps automate the process of downloading videos and images from websites. 

When you type "you-get" command in the terminal, it scans the URL of the video or image provided and then downloads the media file from the website, and saves it into the specified directory. It supports multiple video and image formats, including MP4, WebM, OGG, MP3, JPEG, PNG, and more. 

You-Get is very user-friendly, and you don't need to have any programming skills to use it. To use You-get, you need to first install it on your system. Once you have installed it, run the command followed by the URL of the video or image you want to download.

For example, if you want to download a video from YouTube, you should type the following command:

you-get https://www.youtube.com/watch?v=dQw4w9WgXcQ 

This command will extract the video file and download it to your local directory. It's also possible to specify the output directory with this command, like this:

you-get -O /home/user/Downloads https://www.youtube.com/watch?v=dQw4w9WgXcQ

This command will save the downloaded video to /home/user/Downloads directory on your system. 

## tldr 
 
> Download media contents (videos, audios, images) from the Web.
> More information: <https://you-get.org>.

- Print media information about a specific media on the web:

`you-get --info {{https://example.com/video?id=value}}`

- Download a media from a specific URL:

`you-get {{https://example.com/video?id=value}}`

- Search on Google Videos and download:

`you-get {{keywords}}`

- Download a media to a specific location:

`you-get --output-dir {{path/to/directory}} --output-filename {{filename}} {{https://example.com/watch?v=value}}`

- Download a media using a proxy:

`you-get --http-proxy {{proxy_server}} {{https://example.com/watch?v=value}}`
