# wal-telegram 
## chatgpt 
As an AI language model, I cannot run commands on your computer or device. However, I can explain what the "wal-telegram" command generally does.

"wal-telegram" is a command that is used to customize the appearance of the Telegram messenger window. The "wal" in "wal-telegram" stands for "pywal" which is a tool used for color palette generation and management. The "telegram" in the command specifies that the customization will be applied to the Telegram application.

When you run the "wal-telegram" command, it uses the colors generated by "pywal" to change the colors of the Telegram messenger window, including the background, text, and other elements. This creates a more personalized and visually appealing experience for the user.

Overall, "wal-telegram" is a useful command for those who want to customize the appearance of the Telegram application using "pywal" color palettes. 

## tldr 
 
> Generates themes for Telegram based the colors generated by pywal/wal.
> More information: <https://github.com/guillaumeboehm/wal-telegram>.

- Generate with wal's palette and the current wallpaper (feh only):

`wal-telegram`

- Generate with wal's palette and a specified background image:

`wal-telegram --background={{path/to/image}}`

- Generate with wal's palette and a colored background based on the palette:

`wal-telegram --tiled`

- Apply a gaussian blur on the background image:

`wal-telegram -g`

- Specify a location for the generated theme (default is `$XDG_CACHE_HOME/wal-telegram` or `~/.cache/wal-telegram`):

`wal-telegram --destination={{path/to/destination}}`

- Restart the telegram app after generation:

`wal-telegram --restart`
