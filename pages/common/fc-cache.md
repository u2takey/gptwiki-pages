# fc-cache 
## chatgpt 
The `fc-cache` command is used to build font information cache files for applications that use the Fontconfig library. Fontconfig is a font management library that reduces the work required to access and use fonts. 

The `fc-cache` command scans the directories specified in the `FC\_FONT\_PATH` environment variable as well as the system font directories (/usr/share/fonts, /usr/local/share/fonts, etc.) and creates a cache of available fonts and their attributes. 

When an application requests a font, Fontconfig checks the cache first to see if the font is available before searching through every font in every directory. This reduces the time required to find and load fonts, especially when dealing with large font collections.

Using the `fc-cache` command is typically done after installing or removing fonts on the system. Running `fc-cache -f` will force a full rebuild of the cache, while `fc-cache -v` will print verbose output during the cache building process. 

Overall, the `fc-cache` command is an essential tool for ensuring efficient font loading and management in Linux systems. 

## tldr 
 
> Scan font directories to build font cache files.
> More information: <https://manned.org/fc-cache>.

- Generate font cache files:

`fc-cache`

- Force a rebuild of all font cache files, without checking if cache is up-to-date:

`fc-cache -f`

- Erase font cache files, then generate new font cache files:

`fc-cache -r`
