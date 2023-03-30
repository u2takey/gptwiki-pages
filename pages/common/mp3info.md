# mp3info 
## chatgpt 
The "mp3info" command is a tool used in Linux and Unix operating systems to display information about MP3 audio files. It provides users with details such as the track name, artist name, album name, bit rate, length of the track and other technical specifications of the file. By running the "mp3info" command followed by the name of the MP3 file, users can easily obtain relevant information about that file.

The specifics of the information that is displayed by the "mp3info" command may vary depending on the program's version or the operating system being used. However, common details that are often displayed include the bit rate, sample rate, channel mode, length of the audio file, ID3 tags, and other file-specific technical details.

The "mp3info" command is useful for music enthusiasts who want to get more information about their audio files, especially when managing a large library of music across multiple devices. This command can also be useful for programmers working with audio files in their code, as they can use the "mp3info" command to view the specifications of a file programmatically. 

## tldr 
 
> Viewer/editor for ID3v1 (but not ID3v2) tags of MP3 files.
> More information: <http://www.ibiblio.org/mp3info>.

- Show all ID3v1 tags of a specific MP3 file:

`mp3info {{path/to/file.mp3}}`

- Edit ID3v1 tags interactively:

`mp3info -i {{path/to/file.mp3}}`

- Set values for ID3v1 tags in a specific MP3 file:

`mp3info -a "{{artist_name}}" -t "{{song_title}}" -l "{{album_title}}" -y {{year}} -c "{{comment_text}}" {{path/to/file.mp3}}`

- Set the number of the track in the album for a specific MP3 file:

`mp3info -n {{track_number}} {{path/to/file.mp3}}`

- Print a list of valid genres and their numeric codes:

`mp3info -G`

- Set the music genre for a specific MP3 file:

`mp3info -g {{genre_number}} {{path/to/file.mp3}}`
