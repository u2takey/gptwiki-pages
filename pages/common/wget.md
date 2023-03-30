# wget 
## chatgpt 
The "wget" command is a commonly used tool on Linux and macOS systems that allows you to download files from the internet. The name "wget" stands for "web get" and it is a free utility that works without requiring any user interaction. Some key features and flags of the "wget" command are:

- Basic Syntax: The basic syntax of the "wget" command is as follows: 

  wget [options] [URL]

  You simply need to enter the URL of the file you want to download after the "wget" command, and it will start downloading the file immediately.

- Recursive Download: With the "-r" option, you can instruct "wget" to download all files and sub-directories present on a website. This is useful when you want to download a whole website for offline viewing.

- Download Limits: The "-limit-rate" option allows you to limit the download rate of a file, useful when you want to avoid hogging bandwidth on a shared network.

- Download Resume: With the "-c" option, you can instruct "wget" to resume a previously interrupted download. You can use this option to avoid downloading large files from the beginning if the download has been interrupted.

- Output File: The "-O" option allows you to specify the name of the output file. By default, "wget" will save the downloaded file with the same filename as the one on the server, but you can use this option to give the file a different name.

Overall, "wget" is a versatile and powerful command-line tool that allows you to download files from the internet quickly and efficiently. Its ability to recursively download a website, resume interrupted downloads, and set download limits makes it a valuable tool for system admins and power users. 

## tldr 
 
> Download files from the Web.
> Supports HTTP, HTTPS, and FTP.
> More information: <https://www.gnu.org/software/wget>.

- Download the contents of a URL to a file (named "foo" in this case):

`wget {{https://example.com/foo}}`

- Download the contents of a URL to a file (named "bar" in this case):

`wget --output-document {{bar}} {{https://example.com/foo}}`

- Download a single web page and all its resources with 3-second intervals between requests (scripts, stylesheets, images, etc.):

`wget --page-requisites --convert-links --wait=3 {{https://example.com/somepage.html}}`

- Download all listed files within a directory and its sub-directories (does not download embedded page elements):

`wget --mirror --no-parent {{https://example.com/somepath/}}`

- Limit the download speed and the number of connection retries:

`wget --limit-rate={{300k}} --tries={{100}} {{https://example.com/somepath/}}`

- Download a file from an HTTP server using Basic Auth (also works for FTP):

`wget --user={{username}} --password={{password}} {{https://example.com}}`

- Continue an incomplete download:

`wget --continue {{https://example.com}}`

- Download all URLs stored in a text file to a specific directory:

`wget --directory-prefix {{path/to/directory}} --input-file {{URLs.txt}}`
