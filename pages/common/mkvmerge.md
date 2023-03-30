# mkvmerge 
## chatgpt 
Mkvmerge is a command-line tool used to merge multiple video, audio, subtitle, and other multimedia streams into a single Matroska (MKV) file. Matroska is an open container format that can store various types of multimedia content in a single file, including video, audio, subtitles, and other metadata.

The "mkvmerge" command is used to initiate the process of merging different multimedia streams. The command follows a specific syntax which includes various options and arguments to define the input and output files and specify the settings for the merge process.

Some common options used with the mkvmerge command include:

- -o to specify the output file name and location
- -a to add audio streams to the output file
- -s to add subtitle streams to the output file
- -d to add video streams to the output file
- -T to add tags to the output file for easy indexing and searching

Here's an example of how the mkvmerge command may look like:

mkvmerge -o output.mkv input1.mkv +input2.mkv

This command merges two input files (input1.mkv and input2.mkv) and creates a new output file called output.mkv. The "+" sign between the two input file names indicates that they should be merged rather than concatenated.

There are many other options and arguments that can be used with the mkvmerge command to customize the output file, such as adjusting the audio and video codecs, specifying the language of the audio and subtitle tracks, and adding chapters to the output file. 

## tldr 
 
> Merge and extract multimedia streams.
> More information: <https://mkvtoolnix.download/doc/mkvmerge.html>.

- Display information about a Matroska file:

`mkvmerge --identify {{path/to/file.mkv}}`

- Extract the audio from track 1 of a specific file:

`mkvextract tracks {{path/to/file.mkv}} {{1}}:{{path/to/output.webm}}`

- Extract the subtitle from track 3 of a specific file:

`mkvextract tracks {{path/to/file.mkv}} {{3}}:{{path/to/subs.srt}}`

- Add a subtitle track to a file:

`mkvmerge --output {{path/to/output.mkv}} {{path/to/file.mkv}} {{path/to/subs.srt}}`
