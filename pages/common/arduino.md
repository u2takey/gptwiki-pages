# arduino 
## chatgpt 
The "arduino" command is used to run the Arduino IDE from the command line. It allows users to compile, upload, and monitor Arduino sketches from a terminal window, rather than using the GUI of the Arduino IDE.

Here is a brief explanation of some of the main options and arguments of the arduino command:

- `--board`: the type of Arduino board being used, such as "uno", "mega", "nano", etc.
- `--port`: the serial port to use for communication with the Arduino board.
- `--upload`: compiles the sketch and uploads it to the board.
- `--verify`: compiles the sketch without uploading it.
- `--get-pref`: retrieves a specific preference from the Arduino IDE preferences file.
- `--set-pref`: sets a specific preference in the Arduino IDE preferences file.
- `--preferences-file`: specifies a custom preferences file to use instead of the default.
- `sketch_file`: the path to the sketch file (.ino) that should be compiled and uploaded.

Overall, the arduino command is a useful tool for developers who prefer to work from the command line or who need to automate certain processes. 

## tldr 
 
> Arduino Studio - Integrated Development Environment for the Arduino platform.
> More information: <https://github.com/arduino/Arduino/blob/master/build/shared/manpage.adoc>.

- Build a sketch:

`arduino --verify {{path/to/file.ino}}`

- Build and upload a sketch:

`arduino --upload {{path/to/file.ino}}`

- Build and upload a sketch to an Arduino Nano with an Atmega328p CPU, connected on port `/dev/ttyACM0`:

`arduino --board {{arduino:avr:nano:cpu=atmega328p}} --port {{/dev/ttyACM0}} --upload {{path/to/file.ino}}`

- Set the preference `name` to a given `value`:

`arduino --pref {{name}}={{value}}`

- Build a sketch, put the build results in the build directory, and reuse any previous build results in that directory:

`arduino --pref build.path={{path/to/build_directory}} --verify {{path/to/file.ino}}`

- Save any (changed) preferences to `preferences.txt`:

`arduino --save-prefs`

- Install the latest SAM board:

`arduino --install-boards "{{arduino:sam}}"`

- Install Bridge and Servo libraries:

`arduino --install-library "{{Bridge:1.0.0,Servo:1.2.0}}"`
