# mplayer 
## chatgpt 
MPlayer is a command-line media player program for Linux/Unix, Windows, OSX platforms. It is a software that enables you to play audio and video files directly from the command line. 

Here's how to use the mplayer command:

1. Open the terminal application on your computer.
2. Type "mplayer" followed by the file name and extension in the command line.
3. The player will start playing the media file automatically.

You can use additional parameters available with MPlayer to customize the playback options. Some commonly used parameters are:

- -vo: specifies the video output driver.
- -ao: specifies the audio output driver.
- -sub: loads and displays subtitles.
- -speed: changes the playback speed of the media file.

Overall, MPlayer is a powerful command-line media player that allows playing a wide range of audio and video formats with customization options. 

## tldr 
 
> Cross-platform multimedia player.
> More information: <https://mplayerhq.hu/DOCS/HTML/en/commandline.html>.

- Play the specified file or URL:

`mplayer {{path/to/file|url}}`

- Play multiple files:

`mplayer {{path/to/file1 path/to/file2 ...}}`

- Play a specific file repeatedly:

`mplayer -loop {{0}} {{path/to/file}}`

- Pause playback:

`<Space>`

- Quit mplayer:

`<Escape>`

- Seek backward or forward 10 seconds:

`<Left> or <Right>`
