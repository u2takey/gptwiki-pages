# sox 
## chatgpt 
SoX is a command-line audio processing tool used to convert, edit, and manipulate audio files. Some of the functionalities include:

- Converting audio file formats: SoX can convert audio files from one format to another such as WAV, MP3, FLAC, etc.
- Changing audio properties: SoX can change various audio properties like sample rate, bit depth, etc.
- Adding effects: SoX offers a range of effects that can be applied to audio files such as reverb, echo, chorus, etc.
- Mixing multiple audio files: SoX can mix multiple audio files into one.

To use SoX, the user needs to open the command-line interface on their computer, navigate to the directory where their audio file is saved, and enter the command followed by desired options and parameters. For example, to convert an MP3 file to a WAV file, the command in the terminal would be:

`sox input.mp3 output.wav`

This will result in a converted file called `output.wav` that will be saved in the same directory as the original `input.mp3` file.

Overall, SoX provides a comprehensive set of audio processing tools for users with some command-line experience. 

## tldr 
 
> Sound eXchange: play, record and convert audio files.
> Audio formats are identified by the extension.
> More information: <http://sox.sourceforge.net>.

- Merge two audio files into one:

`sox -m {{input_audiofile1}} {{input_audiofile2}} {{output_audiofile}}`

- Trim an audio file to the specified times:

`sox {{input_audiofile}} {{output_audiofile}} trim {{start}} {{end}}`

- Normalize an audio file (adjust volume to the maximum peak level, without clipping):

`sox --norm {{input_audiofile}} {{output_audiofile}}`

- Reverse and save an audio file:

`sox {{input_audiofile}} {{output_audiofile}} reverse`

- Print statistical data of an audio file:

`sox {{input_audiofile}} -n stat`

- Increase the volume of an audio file by 2x:

`sox -v 2.0 {{input_audiofile}} {{output_audiofile}}`
