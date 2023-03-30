# rtmpdump 
## chatgpt 
rtmpdump is a command-line tool used to stream or download content from media servers using the Real-Time Messaging Protocol (RTMP). It is an open-source application that works on various operating systems, including Windows, Linux, and macOS.

Some of the key features of rtmpdump include:

1. Supports RTMP and RTMPE protocols for streaming or downloading content.
2. Allows users to capture live broadcasting sessions and save them to local storage.
3. Supports multiple media formats, including FLV, MP3, and SWF, etc.
4. Can be used to convert streaming files into other media formats.
5. Supports authentication for protected media files.

To use rtmpdump, you will need to have the URL of the media server and the stream key that correspond to the content you want to access. The basic syntax for the rtmpdump command is:

rtmpdump -r "rtmp://server.com/app/stream" -o filename.flv

This command will stream or download the content from the specified media server and save it to a file named "filename.flv" in the current working directory. The "-r" option is used to specify the URL of the media server, while the "-o" option is used to define the output file name.

In addition to these basic options, rtmpdump also supports a wide range of other parameters that allow users to customize the download or streaming experience. For example, users can specify the buffer size, add a proxy server, and increase the download speed by setting the maximum download bandwidth.

To see a list of all the available options and parameters that can be used with rtmpdump, you can type "rtmpdump --help" into the command prompt. This will display a list of all the available options, including their descriptions and usage examples. 

## tldr 
 
> A tool to dump media content streamed over the RTMP protocol.
> More information: <http://rtmpdump.mplayerhq.hu/>.

- Download a file:

`rtmpdump --rtmp {{rtmp://example.com/path/to/video}} -o {{file.ext}}`

- Download a file from a Flash player:

`rtmpdump --rtmp {{rtmp://example.com/path/to/video}} --swfVfy {{http://example.com/player}} --flashVer "{{LNX 10,0,32,18}}" -o {{file.ext}}`

- Specify connection parameters if they are not detected correctly:

`rtmpdump --rtmp {{rtmp://example.com/path/to/video}} --app {{app_name}} --playpath {{path/to/video}} -o {{file.ext}}`

- Download a file from a server that requires a referrer:

`rtmpdump --rtmp {{rtmp://example.com/path/to/video}} --pageUrl {{http://example.com/webpage}} -o {{file.ext}}`
