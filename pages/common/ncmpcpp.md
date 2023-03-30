# ncmpcpp 
## chatgpt 
ncmpcpp is a command-line based music player for Unix-like systems. It provides an interactive interface for browsing and playing music files. Here's a breakdown of the main features of the ncmpcpp command:

- Navigation: ncmpcpp allows users to navigate through their music library with ease. Users can browse by artist, album, playlist, or genre. They can also search for specific tracks or albums.
- Playback controls: The command supports playback control functions like start, stop, pause, resume, skip forward or backward, shuffle, and repeat.
- Visualization options: ncmpcpp provides various visualization options such as a built-in visualizer that shows the waveform of the current track being played, a spectrum analyzer for analyzing the frequency of the music played, and an oscilloscope to display the sound waves.
- Configuration options: Users can customize ncmpcpp by editing the configuration file. This file is usually located in the ~/.ncmpcpp directory, and it contains settings that allow users to configure the command-line interface, adjust the audio output, and set the default database file.
- Keybindings: ncmpcpp allows users to bind keys to various commands. This can help streamline the control of the music player, making it more efficient to use.
- Integration with other music players: ncmpcpp can be integrated with other music players like MPD (Music Player Daemon) by accessing MPD's database files and playing music from there.

In summary, ncmpcpp is a powerful command-line based music player that provides users with a feature-rich interface, advanced playback controls, and customization options. 

## tldr 
 
> A command-line music player client for the Music Player Daemon.
> More information: <https://rybczak.net/ncmpcpp>.

- Connect to a music player daemon on a given host and port:

`ncmpcpp --host {{ip}} --port {{port}}`

- Display metadata of the current song to console:

`ncmpcpp --current-song`

- Use a specified configuration file:

`ncmpcpp --config {{file}}`

- Use a different set of key bindings from a file:

`ncmpcpp --bindings {{file}}`
