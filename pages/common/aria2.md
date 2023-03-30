# aria2 
## chatgpt 
Aria2 is a command-line based download manager program that can be used to download files of various types and sizes over multiple protocols such as HTTP, FTP, SFTP, BitTorrent, and Metalink. 

The command for using Aria2 is simply "aria2" followed by a series of options and/or URLs to the files you want to download. Here's an example command:

```
aria2c -s 10 -x 16 http://example.com/file.mp4
```

- `aria2c` is an alias for `aria2`, used to invoke the program.
- `-s 10` specifies the number of connections to use for the download. In this case, we're using 10 connections.
- `-x 16` specifies the maximum number of simultaneous connections per server. In this case, we're using 16 connections.
- `http://example.com/file.mp4` is the URL of the file we want to download.

Other common options that can be used with aria2 include:

- `-o` followed by the name of the output file. For example: `-o myvideo.mp4`
- `-d` followed by the path to the directory where the file should be saved. For example: `-d /home/user/downloads/`
- `-u` followed by the username for authentication, if required. For example: `-u username`
- `-p` followed by the password for authentication. For example: `-p password`
- `-h` to see a list of available options and commands.

Overall, aria2 is a powerful and flexible download manager that can greatly simplify the process of downloading files from the internet. 

## tldr 
 
> This command is an alias of `aria2c`.

- View documentation for the updated command:

`tldr aria2c`
