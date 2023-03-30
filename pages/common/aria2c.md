# aria2c 
## chatgpt 
aria2c is a command-line download utility that allows downloading files using various protocols such as HTTP, FTP, BitTorrent, and Metalink. Here's the explanation of the command:

- `aria2c` - The name of the command used for initiating downloads
- `-S` - Used to check the availability of file sources before download
- `-o` - Used to specify the name and location of the output file
- `-x` - Used to limit the maximum number of connections to a server for a single download
- `-s` - Used to set the number of segments per download
- `-d` - Used to specify the download directory
- `<URL>` - The URL of the file that needs to be downloaded

For example, to download a file named "example.zip" from a URL https://example.com/example.zip using aria2c with four connections per server and a total of eight segments, the command would look like this:

```
aria2c -S -x 4 -s 8 -d /home/user/Downloads/ -o example.zip https://example.com/example.zip
```

This will initiate the download of the file "example.zip" to the directory /home/user/Downloads/ with four connections per server and a total of eight segments. 

## tldr 
 
> Fast download utility.
> Supports HTTP(S), FTP, SFTP, BitTorrent, and Metalink.
> More information: <https://aria2.github.io>.

- Download a specific URI to a file:

`aria2c "{{url}}"`

- Download a file from a URI with a specific output name:

`aria2c --out={{path/to/file}} "{{url}}"`

- Download multiple different files in parallel:

`aria2c --force-sequential {{false}} "{{url1 url2 ...}}"`

- Download from multiple sources with each URI pointing to the same file:

`aria2c "{{url1 url2 ...}}"`

- Download the URIs listed in a file with a specific number of parallel downloads:

`aria2c --input-file={{path/to/file}} --max-concurrent-downloads={{number_of_downloads}}`

- Download with multiple connections:

`aria2c --split={{number_of_connections}} "{{url}}"`

- FTP download with username and password:

`aria2c --ftp-user={{username}} --ftp-passwd={{password}} "{{url}}"`

- Limit download speed in bytes/s:

`aria2c --max-download-limit={{speed}} "{{url}}"`
