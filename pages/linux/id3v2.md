# id3v2 
## chatgpt 
The "id3v2" command is a command-line utility that is used to manipulate and manage the version 2 of ID3 tags in audio files. ID3 tags are metadata tags that can be embedded in audio files, such as MP3s, to provide additional information about the audio contents, such as artist name, album name, track number, and genre.

The "id3v2" command can be used to perform a variety of tasks related to ID3 tags, including adding, modifying, and removing tags. Some of the common command options and their uses are:

- -l: List the ID3 tags in a specified audio file
- -A: Set the album name tag value
- -T: Set the track number tag value
- -a: Set the artist name tag value
- -t: Set the title tag value
- -g: Set the genre tag value
- -c: Set the comment tag value
- -y: Set the year tag value
- -I: Set the unique file identifier tag value

Example usage:

To view the ID3 tags of an audio file named "song.mp3":

id3v2 -l song.mp3

To set the artist name tag value to "John Doe" for the same file:

id3v2 -a "John Doe" song.mp3

Overall, the "id3v2" command is a useful tool for managing ID3 tags in audio files, and it can greatly enhance the organization and user experience of a digital music library. 

## tldr 
 
> Manages id3v2 tags, converts and lists id3v1.
> More information: <https://manned.org/id3v2.1>.

- List all genres:

`id3v2 ‐‐list‐genres`

- List all tags of specific files:

`id3v2 --list-tags {{path/to/file1 path/to/file2 ...}}`

- Delete all `id3v2` or `id3v1` tags of specific files:

`id3v2 {{--delete‐v2|--delete‐v1}} {{path/to/file1 path/to/file2 ...}}`

- Display help:

`id3v2 --help`

- Display version:

`id3v2 ‐‐version`
