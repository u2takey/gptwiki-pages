# aplay 
## chatgpt 
`aplay` is a command-line tool used to play audio files on a Linux system. It is a part of the ALSA (Advanced Linux Sound Architecture), which provides audio drivers for Linux systems. 

Syntax: ```aplay [OPTIONS] [FILE]```

Here, 
- `OPTIONS`: It specifies various options such as the audio device, format, and sample rate to use while playing the audio file.
- `FILE`: It specifies the audio file to be played.

Example: 
```aplay sample.wav```

This command will play the audio file `sample.wav` using the default audio device and settings.

OPTIONS:
- `-D`: It specifies the audio device to use for playback. 
  Example: `aplay -D hw:0 sample.wav` will play the audio file using the first audio device (`hw:0`).
  
- `-f`: It specifies the audio format to use.
  Example: `aplay -f cd sample.wav` will play the audio file using CD quality format.
  
- `-r`: It specifies the sample rate to use.
  Example: `aplay -r 48000 sample.wav` will play the audio file using a sample rate of 48 kHz.
  
By default, `aplay` will play the audio file using the system's default audio device and settings. It supports various audio file formats such as WAV, AIFF, AU, and raw audio data. 

## tldr 
 
> Command-line sound player for ALSA soundcard driver.
> More information: <https://manned.org/aplay>.

- Play a specific file (sampling rate, bit depth, etc. will be automatically determined for the file format):

`aplay {{path/to/file}}`

- Play the first 10 seconds of a specific file at 2500 Hz:

`aplay --duration={{10}} --rate={{2500}} {{path/to/file}}`

- Play the raw file as a 22050 Hz, mono, 8-bit, Mu-Law `.au` file:

`aplay --channels={{1}} --file-type {{raw}} --rate={{22050}} --format={{mu_law}} {{path/to/file}}`
