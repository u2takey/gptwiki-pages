# eyeD3 
## chatgpt 
eyeD3 is a command-line tool and Python library for working with audio files, specifically MP3 files. It allows you to view information about the file, such as ID3 tags, and edit or add new ones.

There are a variety of commands you can use with eyeD3, depending on the action you want to perform. Here are a few examples:

1. `eyeD3 --info file.mp3` - This command displays information about the MP3 file, including its bitrate, duration, and ID3 tags.

2. `eyeD3 --set-artist="John Smith" file.mp3` - This command sets the artist tag for the specified MP3 file to "John Smith."

3. `eyeD3 --remove-comments file.mp3` - This command removes any comments that have been added to the file's ID3 tags.

4. `eyeD3 --rename="%n %t" *.mp3` - This command renames all MP3 files in the current directory according to a specified format. In this example, the new name will consist of the track number followed by the title.

It's worth noting that eyeD3 is not limited to working with MP3 files, though that is its primary focus. It can also handle other audio file formats like FLAC and Ogg Vorbis. 

## tldr 
 
> Read and manipulate metadata of MP3 files.
> More information: <https://eyed3.readthedocs.io>.

- View information about an MP3 file:

`eyeD3 {{filename.mp3}}`

- Set the title of an MP3 file:

`eyeD3 --title "{{A Title}}" {{filename.mp3}}`

- Set the album of all the MP3 files in a directory:

`eyeD3 --album "{{Album Name}}" {{*.mp3}}`

- Set the front cover art for an MP3 file:

`eyeD3 --add-image {{front_cover.jpeg}}:FRONT_COVER: {{filename.mp3}}`
