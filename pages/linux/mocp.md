# mocp 
## chatgpt 
The 'mocp' command stands for Music On Console Player. It is a text-based audio player for Linux and Unix-based operating systems. 

When you run the 'mocp' command, it opens a console-based interface that allows you to play, pause, stop, and navigate through your music collection. It supports a wide range of audio formats including MP3, OGG, FLAC, WAV, and more. 

Here are some of the basic commands you can use when running the 'mocp' command:

- 'mocp -S' will start the player and scan your music directory for audio files. 
- 'mocp' (without any parameters) will launch the player interface. 
- 'mocp -p' will toggle between play and pause. 
- 'mocp --next' will skip to the next track in the playlist. 
- 'mocp --prev' will skip to the previous track in the playlist. 
- 'mocp --stop' will stop playback. 

You can also use the 'mocp' interface to create and manage playlists, adjust volume settings, and customize other aspects of the player's functionality. 

## tldr 
 
> Music on Console (MOC) audio player.
> More information: <https://manned.org/mocp>.

- Launch the MOC terminal UI:

`mocp`

- Launch the MOC terminal UI in a specific directory:

`mocp {{path/to/directory}}`

- Start the MOC server in the background, without launching the MOC terminal UI:

`mocp --server`

- Add a specific song to the play queue while MOC is in the background:

`mocp --enqueue {{path/to/audio_file}}`

- Add songs recursively to the play queue while MOC is in the background:

`mocp --append {{path/to/directory}}`

- Clear the play queue while MOC is in the background:

`mocp --clear`

- Play or stop the currently queued song while MOC is in the background:

`mocp --{{play|stop}}`

- Stop the MOC server while it's in the background:

`mocp --exit`
