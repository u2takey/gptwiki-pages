# musescore 
## chatgpt 
Musescore is a command that launches the software application MuseScore. MuseScore is a music notation software that is used to create, edit, and print music scores. It offers a variety of tools and features that allow users to write sheet music for a range of instruments and ensembles. These tools include note input, editing, playback, and printing options. The command "musescore" launches the software and allows the user to start creating or editing a musical score. It can be used in a terminal or command prompt on various operating systems such as Windows, macOS, and Linux. 

## tldr 
 
> MuseScore 3 sheet music editor.
> More information: <https://musescore.org/en/handbook/3/command-line-options>.

- Use a specific audio driver:

`musescore --audio-driver {{jack|alsa|portaudio|pulse}}`

- Set the MP3 output bitrate in kbit/s:

`musescore --bitrate {{bitrate}}`

- Start MuseScore in debug mode:

`musescore --debug`

- Enable experimental features, such as layers:

`musescore --experimental`

- Export the given file to the specified output file. The file type depends on the given extension:

`musescore --export-to {{output_file}} {{input_file}}`

- Print a diff between the given scores:

`musescore --diff {{path/to/file1}} {{path/to/file2}}`

- Specify a MIDI import operations file:

`musescore --midi-operations {{path/to/file}}`
