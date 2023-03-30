# id3tag 
## chatgpt 
id3tag is a command-line utility that lets you edit the ID3 tags of audio files. ID3 tags are meta data that contain information about the audio file such as the song title, artist name, album title, and genre. 

The id3tag command has various options that allow you to modify, view, and remove ID3 tags. Here are some of the basic options:

1. -l, --list: This option lists the current ID3 tags of a file.

Example: `id3tag -l audiofile.mp3`

2. -a, --artist: This option sets the artist name of a file.

Example: `id3tag -a "New Artist" audiofile.mp3`

3. -t, --title: This option sets the title of a file.

Example: `id3tag -t "New Title" audiofile.mp3`

4. -A, --album: This option sets the album name of a file.

Example: `id3tag -A "New Album" audiofile.mp3`

5. -g, --genre: This option sets the genre of a file.

Example: `id3tag -g "Rock" audiofile.mp3`

6. -y, --year: This option sets the year of a file.

Example: `id3tag -y "1995" audiofile.mp3`

7. -c, --comment: This option sets a comment for a file.

Example: `id3tag -c "This is a great song" audiofile.mp3`

8. --remove-v1: This option removes the ID3v1 tag from a file.

Example: `id3tag --remove-v1 audiofile.mp3`

9. --remove-v2: This option removes the ID3v2 tag from a file.

Example: `id3tag --remove-v2 audiofile.mp3`

Overall, the id3tag command is a useful tool for managing your audio file metadata. 

## tldr 
 
> Tool for reading, writing, and manipulating ID3v1 and ID3v2 tags of MP3 files.
> More information: <https://manned.org/id3tag>.

- Set artist and title tag of an MP3 file:

`id3tag --artist={{artist}} --title={{title}} {{path/to/file.mp3}}`

- Set album title of all MP3 files in the current directory:

`id3tag --album={{album}} {{*.mp3}}`

- Get more help:

`id3tag --help`
