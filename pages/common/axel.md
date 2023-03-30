# axel 
## chatgpt 
Axel is a Linux command-line utility that allows users to download files from the Internet with speed and efficiency, using multiple connections. With axel, you can speed up your downloads by splitting a file into multiple segments, which are then downloaded simultaneously.

To use the `axel` command, you would typically start by opening a terminal window in Linux. You then need to specify the URL of the file you want to download, along with any options you want to use, such as the number of connections to use or the output directory.

Here is the basic syntax of the `axel` command:

```
axel [OPTIONS] URL
```

Here are some of the most common options you can use with the `axel` command:

- `-n`: specifies the number of connections to use (default is 8)
- `-o`: specifies the output filename or directory
- `-s`: specifies the size of each segment in bytes (default is 1048576 bytes, or 1 MB)
- `-a`: specifies the user-agent string to use in the HTTP header
- `-v`: enables verbose output

For example, to download a file with axel, you might use the following command:

```
axel -n 10 http://example.com/file.zip
```

This would download the file `file.zip` from `http://example.com` using 10 connections.

Overall, the `axel` command is a powerful tool for downloading files quickly and efficiently in Linux. 

## tldr 
 
> Download accelerator.
> Supports HTTP, HTTPS, and FTP.
> More information: <https://github.com/axel-download-accelerator/axel>.

- Download a URL to a file:

`axel {{url}}`

- Download and specify filename:

`axel {{url}} -o {{path/to/file}}`

- Download with multiple connections:

`axel -n {{connections_num}} {{url}}`

- Search for mirrors:

`axel -S {{mirrors_num}} {{url}}`

- Limit download speed (bytes per second):

`axel -s {{speed}} {{url}}`
