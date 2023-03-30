# arecord 
## chatgpt 
The `arecord` command is a Linux-based command-line tool that is used for recording audio from a connected capture device such as a microphone or a line-in input jack. It is available on most Linux distributions and is part of the ALSA (Advanced Linux Sound Architecture) sound system.

The `arecord` command provides a flexible way to capture audio input and save it in a variety of formats, including PCM (Pulse Code Modulation) or WAV (Windows Audio File Format). It can also be used with a number of different options, allowing users to adjust parameters such as the recording quality, input source, and recording duration.

Some common use cases for `arecord` include capturing audio for voiceover work, creating podcasts, or simply recording sound bites or snippets for personal or professional use. Its versatility and highly configurable nature make it a popular choice for Linux users who need to record audio on a regular basis. 

## tldr 
 
> Sound recorder for ALSA soundcard driver.
> More information: <https://manned.org/arecord>.

- Record a snippet in "CD" quality (finish with Ctrl-C when done):

`arecord -vv --format=cd {{path/to/file.wav}}`

- Record a snippet in "CD" quality, with a fixed duration of 10 seconds:

`arecord -vv --format=cd --duration={{10}} {{path/to/file.wav}}`

- Record a snippet and save it as an MP3 (finish with Ctrl-C when done):

`arecord -vv --format=cd --file-type raw | lame -r - {{path/to/file.mp3}}`

- List all sound cards and digital audio devices:

`arecord --list-devices`

- Allow interactive interface (e.g. use space-bar or enter to play or pause):

`arecord --interactive`
