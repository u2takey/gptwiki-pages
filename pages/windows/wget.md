# wget 
## chatgpt 
The 'wget' command is a Linux utility used for downloading files from the internet. It stands for "web get," and it is commonly installed on Unix-based operating systems like Linux and macOS.

The basic syntax of the 'wget' command is as follows:

```
wget [options] [URL]
```

Options are used to modify the behavior of the command, and the URL specifies the file to download.

Here are some commonly used options:

- '-O [filename]': saves the downloaded file with the specified name
- '-q': runs the command in quiet mode, which suppresses output messages
- '-r': recursively downloads the file(s) specified in the URL and all of its linked content
- '-c': resumes a partially downloaded file
- '-b': runs the command in the background so the user can continue to use the terminal

The 'wget' command is often used in shell scripts for automatic fetching and updating of files. It can also be used to download entire websites for offline viewing, as well as for downloading large files that may be prone to interruptions or network issues. 

## tldr 
 
> In PowerShell, this command may be an alias of `Invoke-WebRequest` when the original `wget` program (<https://www.gnu.org/software/wget>) is not properly installed.

- Check whether `wget` is properly installed by printing its version number. If this command evaluates into an error, PowerShell may have substituted this command with `Invoke-WebRequest`:

`curl --version`

- View documentation for the original `wget` command:

`tldr wget -p common`

- View documentation for the original `wget` command in older versions of `tldr` command-line client:

`tldr wget -o common`

- View documentation for PowerShell's `Invoke-WebRequest` command:

`tldr invoke-webrequest`
