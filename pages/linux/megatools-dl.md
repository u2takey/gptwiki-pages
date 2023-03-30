# megatools-dl 
## chatgpt 
The "megatools-dl" command is used to download files from the MEGA cloud storage service. This command is a part of the "megatools" package, which provides various command-line tools for interacting with MEGA. 

When you use the "megatools-dl" command, you need to specify the URL or file identifier of the file you want to download, as well as some optional parameters to control the download. Here are some of the common parameters:

- "--path": specifies the local directory where the downloaded file should be saved. By default, the file is saved in the current directory.
- "--username": specifies the MEGA account username to use for the download. If you don't specify this parameter, the tool will prompt you to enter the username interactively.
- "--password": specifies the MEGA account password to use for the download. If you don't specify this parameter, the tool will prompt you to enter the password interactively.
- "--limit-rate": limits the download speed to the specified rate (in bytes per second). This can be useful if you want to avoid using too much bandwidth or if you have a slow Internet connection.

Once you have specified the required parameters, you can run the "megatools-dl" command to start the download. The tool will connect to the MEGA servers, authenticate with your account, and download the file to your local computer. The progress of the download is displayed in the terminal window, and you can use Ctrl+C to cancel the download if needed. 

## tldr 
 
> Download files from `mega.nz`.
> Part of the `megatools` suite.
> More information: <https://megatools.megous.com/man/megatools-dl.html>.

- Download files from a `mega.nz` link into the current directory:

`megatools-dl {{https://mega.nz/...}}`

- Download files from a `mega.nz` link into a specific directory:

`megatools-dl --path {{path/to/directory}} {{https://mega.nz/...}}`

- Interactively choose which files to download:

`megatools-dl --choose-files {{https://mega.nz/...}}`

- Limit the download speed in KiB/s:

`megatools-dl --limit-speed {{speed}} {{https://mega.nz/...}}`
