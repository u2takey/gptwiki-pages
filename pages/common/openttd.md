# openttd 
## chatgpt 
Openttd is a command used to launch the OpenTTD (Open Transport Tycoon Deluxe) game. OpenTTD is a free and open-source simulation game, which allows players to build and manage a transportation network, including trains, buses, trucks, ships, and airplanes. 

When the "openttd" command is executed, the game is launched on the computer. The user can then start a new game or load a saved game. The game interface opens, which allows the user to create and manage a transportation network, build stations, vehicles, roads, and rails, and compete with other companies to transport passengers and cargo.

OpenTTD provides various game settings and options that can be configured before starting the game. For example, the player can choose the game mode, difficulty level, map size, landscape, economy, and other game settings.

Overall, the "openttd" command is a simple and straightforward command that launches the OpenTTD game, providing a fun and challenging way to simulate transportation management. 

## tldr 
 
> Open source clone of the Microprose game "Transport Tycoon Deluxe".
> More information: <https://www.openttd.org>.

- Start a new game:

`openttd -g`

- Load save game at start:

`openttd -g {{path/to/file}}`

- Start with the specified window resolution:

`openttd -r {{1920x1080}}`

- Start with a custom configuration file:

`openttd -c {{path/to/file}}`

- Start with selected video, sound, and music drivers:

`openttd -v {{video_driver}} -s {{sound_driver}} -m {{music_driver}}`

- Start a dedicated server, forked in the background:

`openttd -f -D {{host}}:{{port}}`

- Join a server with a password:

`openttd -n {{host}}:{{port}}#{{player_name}} -p {{password}}`
