# mpd 
## chatgpt 
The command "mpd" is a command to start the Music Player Daemon (MPD) on a Linux system. 

Music Player Daemon (MPD) is a flexible and powerful music player server that runs in the background. It can play local music files or stream music from various sources, including online radio stations, remote servers, and more. 

When you run the "mpd" command from the terminal, the MPD server is started, and you can then use a client program to connect to the server and manage your music library, playlists, and playback options.

The MPD server can be controlled using various clients such as:

1. Command line interface (CLI)
2. Graphical user interface (GUI)
3. Web interfaces

The main advantage of MPD is its flexibility, which enables users to customize the server to their liking. Users can adjust the playback behavior to match their hardware setup and can manage their music library at any time. MPD supports a wide range of audio formats, and the user can configure it to support more formats by adding suitable plugins. 

In summary, the "mpd" command is used to start the MPD server on your system, allowing you to access and manage your music library through various clients. 

## tldr 
 
> Music Player Daemon.
> More information: <https://www.musicpd.org/>.

- Start MPD:

`mpd`

- Start MPD but don't read from the configuration file:

`mpd --no-config`

- Start MPD and don't detach it from the console:

`mpd --no-daemon`

- Kill the currently running MPD session:

`mpd --kill`
