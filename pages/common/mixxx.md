# mixxx 
## chatgpt 
Mixxx is an open-source DJ software that provides everything you need to perform live mixes using your digital music library. It is a powerful tool that can be used for mixing, scratch, looping, hot cues, and other professional DJ features. The following are some of the command-line options available for Mixxx:

- mixxx: This command launches the Mixxx DJ software.
- --midi-debug: This option enables debug output for MIDI input and output.
- --controller-script: This option loads a specific controller script for the Mixxx software.
- --configdir: This option specifies a custom configuration directory for Mixxx.
- --log-level: This option sets the log level for Mixxx output.
- --version: This option displays the version number of Mixxx.

Overall, Mixxx is a versatile and customizable DJ software that can be used to create a unique and professional DJ experience. Its command-line options allow for greater control and customization of the software to suit your specific needs. 

## tldr 
 
> Free and open source cross-platform DJ software.
> More information: <https://mixxx.org/manual/latest/chapters/appendix.html#command-line-options>.

- Start the Mixxx GUI in fullscreen:

`mixxx --fullScreen`

- Start in safe developer mode to debug a crash:

`mixxx --developer --safeMode`

- Debug a malfunction:

`mixxx --debugAssertBreak --developer --loglevel trace`

- Start Mixxx using the specified settings file:

`mixxx --resourcePath {{mixxx/res/controllers}} --settingsPath {{path/to/settings-file}}`

- Debug a custom controller mapping:

`mixxx --controllerDebug --resourcePath {{path/to/mapping-directory}}`

- Show command-line help:

`mixxx --help`
