# grip 
## chatgpt 
Grip is a command line tool that allows you to rip audio CDs, encode MP3s, Ogg Vorbis, FLAC and other audio formats. The grip command can be used to configure and run the Grip interface. 

Here are some of the common parameters used with the grip command:

- -c or --config: Specifies the location of the configuration file. It allows you to create, edit and save configuration files
- -d or --device: Specifies the CD-ROM device, for example /dev/cdrom
- -M or --manual: Displays the Grip manual page
- -t or --track: Specifies which tracks to rip
- -F or --format: Specifies the audio file format
- -D or --directory: Specifies the output directory for ripped audio files
- -E or --encoder: Specifies the audio encoder to use
- -X or --extra-encoder-options: Specifies additional options for the audio encoder
- -n or --no-cddb: Disables CDDB lookup
- -h or --help: Displays the help message for the grip command
- -V or --version: Displays the version number of Grip. 

Overall, the grip command provides a powerful and flexible way to rip audio CDs and convert audio files. 

## tldr 
 
> Preview GitHub-flavoured Markdown files locally.
> More information: <https://github.com/joeyespo/grip>.

- Start the server and serve the rendered `README` file of a current directory:

`grip`

- Start the server and serve a specific Markdown file:

`grip {{path/to/file.md}}`

- Start the server and open the `README` file of the current directory in the browser:

`grip --browser`

- Start the server in the specified port and serve the rendered `README` file of the current directory:

`grip {{port}}`
