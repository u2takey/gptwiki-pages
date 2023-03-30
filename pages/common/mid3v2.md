# mid3v2 
## chatgpt 
`mid3v2` is a command-line tool used to edit metadata tags (ID3 tags) in audio files. The tool is mainly used to change or add metadata in MP3 audio files. Here’s a detailed breakdown of the command and its parameters:

Command:

`mid3v2`

Parameters:

- `-h` or `--help`: displays a summary of the command’s usage and options.
- `-V` or `--version`: displays the version of the tool.
- `-l` or `--list`: displays the metadata tags present in the audio file.
- `-D` or `--delete-all`: deletes all metadata tags in the audio file.
- `-a` or `--artist`: adds or changes the artist name.
- `-A` or `--album`: adds or changes the album name.
- `-t` or `--song`: adds or changes the song title.
- `-T` or `--track`: adds or changes the track number.
- `-d` or `--date`: adds or changes the release date.
- `-g` or `--genre`: adds or changes the genre.
- `-c` or `--comment`: adds or changes the comment.
- `-y` or `--year`: adds or changes the year of the recording.

Example usage:

`mid3v2 -a "Led Zeppelin" -A "IV" -t "Stairway to Heaven" -T "1" -d "1971" -g "Rock" -c "Greatest rock song ever!" -y "1970s" song.mp3`

This command will set the artist to "Led Zeppelin", album to "IV", song title to "Stairway to Heaven", track number to "1", release date to "1971", genre to "Rock", comment to "Greatest rock song ever!", and year to "1970s", in the audio file named "song.mp3". 

## tldr 
 
> Edit audio tags.
> See also: `id3v2`.
> More information: <https://manned.org/mid3v2.1>.

- List all supported ID3v2.3 or ID3v2.4 frames and their meanings:

`id3v2 --list-frames {{path/to/file1.mp3 path/to/file2.mp3 ...}}`

- List all supported ID3v1 numeric genres:

`id3v2 --list-genres {{path/to/file1.mp3 path/to/file2.mp3 ...}}`

- List all tags in specific files:

`id3v2 --list {{path/to/file1.mp3 path/to/file2.mp3 ...}}`

- Set specific artist, album, or song information:

`id3v2 {{--artist|--album|--song}}={{string}} {{path/to/file1.mp3 path/to/file2.mp3 ...}}`

- Set specific picture information:

`id3v2 --picture={{filename:description:image_type:mime_type}} {{path/to/file1.mp3 path/to/file2.mp3 ...}}`

- Set specific year information:

`id3v2 --year={{YYYY}} {{path/to/file1.mp3 path/to/file2.mp3 ...}}`

- Set specific date information:

`id3v2 --date={{YYYY-MM-DD}} {{path/to/file1.mp3 path/to/file2.mp3 ...}}`
