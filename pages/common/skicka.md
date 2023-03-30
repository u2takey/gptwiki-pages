# skicka 
## chatgpt 
As an AI language model, I don't have access to your system or local environment to provide the exact details of the "skicka" command. However, let me provide some generic information about the command.

"skicka" is a command-line tool (a program that runs on a command-line interface) for the Google Drive cloud storage service. It is used to upload, download, and manage files and folders in your Google Drive account from the terminal.

Here are some basic usage examples of the "skicka" command:

- To upload a local file to your Google Drive account:

    skicka upload /path/to/local/file.pdf /remote/directory/in/drive/

- To sync a local folder to your Google Drive account:

    skicka sync /path/to/local/folder/ /remote/directory/in/drive/

- To list the contents of a remote directory in your Google Drive account:

    skicka ls /remote/directory/in/drive/

- To download a file from your Google Drive account:

    skicka download /remote/directory/in/drive/file.pdf /path/to/local/folder/

There are many other options and functionalities of the "skicka" command. You can check the official documentation and help pages for more information. 

## tldr 
 
> Manage your Google Drive.
> More information: <https://github.com/google/skicka>.

- Upload a file/folder to Google Drive:

`skicka upload {{path/to/local}} {{path/to/remote}}`

- Download a file/folder from Google Drive:

`skicka download {{path/to/remote}} {{path/to/local}}`

- List files:

`skicka ls {{path/to/folder}}`

- Show amount of space used by children folders:

`skicka du {{path/to/parent/folder}}`

- Create a folder:

`skicka mkdir {{path/to/folder}}`

- Delete a file:

`skicka rm {{path/to/file}}`
