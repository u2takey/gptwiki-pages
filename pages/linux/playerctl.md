# playerctl 
## chatgpt 
Playerctl is a command-line utility that allows you to control media players from the terminal. This tool supports a wide range of media players such as Spotify, VLC, Rhythmbox, Audacious, and many others.

The command syntax for playerctl is as follows:

playerctl [command] [options] [args]

Here, the [command] specifies the action you want to perform, [options] are the different parameters you can pass with the command, and [args] are the arguments that the command takes.

Some of the most commonly used playerctl commands are:

1. Play - This command starts playing the media if it's paused or stopped.
Syntax: playerctl play

2. Pause - This command pauses the media if it's playing.
Syntax: playerctl pause

3. Stop - This command stops the media playback.
Syntax: playerctl stop

4. Next - This command plays the next track in the playlist.
Syntax: playerctl next

5. Previous - This command plays the previous track in the playlist.
Syntax: playerctl previous

6. Position - This command shows the current position of the media playback.
Syntax: playerctl position

7. Volume - This command shows the current volume level.
Syntax: playerctl volume

Playerctl also has several options that you can use with the commands to customize their behavior. For example, you can specify the media player you want to control, set a specific volume level, shuffle the playlist, or repeat the current track.

Overall, playerctl is a handy utility for users who prefer using the command-line interface to control their media players. 

## tldr 
 
> Utility to control different media players.
> More information: <https://github.com/altdesktop/playerctl>.

- Toggle play:

`playerctl play-pause`

- Next media:

`playerctl next`

- Previous media:

`playerctl previous`

- List all players:

`playerctl --list-all`

- Send a command to a specific player:

`playerctl --player={{player_name}} {{command}}`

- Send a command to all players:

`playerctl --all-players {{command}}`

- Show now playing:

`playerctl metadata --format "Now playing: {{artist}} - {{album}} - {{title}}"`
