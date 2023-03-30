# yt-dlp 
## chatgpt 
yt-dlp is a command-line program that is used to download videos and audio from various websites such as YouTube, Vimeo, and Dailymotion. It is an extension of a popular media downloader known as youtube-dl. The yt-dlp program has additional features and improvements in terms of download speed, UI, and compatibility with different platforms compared to youtube-dl.

To use yt-dlp, you first need to install it on your system. It is available for Windows, macOS, and Linux operating systems. Once installed, you can open the command-line interface on your system and type the command "yt-dlp," followed by the URL of the video or audio that you want to download.

For example, to download a video from YouTube using yt-dlp, you can type the following command:

yt-dlp https://www.youtube.com/watch?v=dQw4w9WgXcQ

This will download the video with the ID "dQw4w9WgXcQ" from YouTube into your current working directory.

The program also offers various options that you can use to customize your downloads such as selecting a specific video quality, downloading only the audio, or downloading subtitles. You can find a full list of available options by typing "yt-dlp --help" in your command-line interface.

Overall, yt-dlp is a versatile and powerful tool for downloading media from various websites, and it can save you time and effort compared to using a web browser or other media downloading tools. 

## tldr 
 
> A youtube-dl fork with additional features and fixes.
> Download videos from YouTube and other websites.
> More information: <https://github.com/yt-dlp/yt-dlp>.

- Download a video or playlist (with the default options from command below):

`yt-dlp "{{https://www.youtube.com/watch?v=oHg5SJYRHA0}}"`

- List the available downloadable formats for a video:

`yt-dlp --list-formats "{{https://www.youtube.com/watch?v=oHg5SJYRHA0}}"`

- Download a video with a defined format, in this case the best mp4 video available (default is "bv\*+ba/b"):

`yt-dlp --format "{{bv*[ext=mp4]+ba[ext=m4a]/b[ext=mp4]}}" "{{https://www.youtube.com/watch?v=oHg5SJYRHA0}}"`

- Extract audio from a video (requires ffmpeg or ffprobe):

`yt-dlp --extract-audio "{{https://www.youtube.com/watch?v=oHg5SJYRHA0}}"`

- Specify audio format and audio quality of extracted audio (between 0 (best) and 10 (worst), default = 5):

`yt-dlp --extract-audio --audio-format {{mp3}} --audio-quality {{0}} "{{https://www.youtube.com/watch?v=oHg5SJYRHA0}}"`

- Download all playlists of YouTube channel/user keeping each playlist in separate directory:

`yt-dlp -o "{{%(uploader)s/%(playlist)s/%(playlist_index)s - %(title)s.%(ext)s}}" "{{https://www.youtube.com/user/TheLinuxFoundation/playlists}}"`

- Download Udemy course keeping each chapter in separate directory under MyVideos directory in your home:

`yt-dlp -u {{user}} -p {{password}} -P "{{~/MyVideos}}" -o "{{%(playlist)s/%(chapter_number)s - %(chapter)s/%(title)s.%(ext)s}}" "{{https://www.udemy.com/java-tutorial}}"`

- Download entire series season keeping each series and each season in separate directory under C:/MyVideos:

`yt-dlp -P "{{C:/MyVideos}}" -o "{{%(series)s/%(season_number)s - %(season)s/%(episode_number)s - %(episode)s.%(ext)s}}" "{{https://videomore.ru/kino_v_detalayah/5_sezon/367617}}"`
