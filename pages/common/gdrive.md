# gdrive 
## chatgpt 
The `gdrive` command is a command-line tool for Google Drive that allows users to interact with their Google Drive files and folders directly from the command line. 

With `gdrive`, users can perform various operations such as:

- Uploading and downloading files.
- Creating and managing folders.
- Sharing files and folders with other users.
- Searching and listing files and folders.
- and much more.

To use `gdrive` command, users need to first authenticate their Google account with the command-line tool by creating an OAuth client ID and secret, following the instructions given by the tool. 

Once authenticated, users can then use the `gdrive` command followed by the operation they wish to perform and the necessary parameters, flags, or options if required.

Here are some examples of how to use `gdrive` command:

- `gdrive upload path/to/file`: This command uploads a file located at "path/to/file" to the user's Google Drive.
- `gdrive share fileID user@example.com`: This command shares a file identified by "fileID" with the email address "user@example.com".
- `gdrive list -q "name contains 'test'"`: This command lists all files and folders in the user's Google Drive that have the word "test" in their names.

Overall, `gdrive` is a powerful command-line tool for managing and interacting with Google Drive that can boost productivity for users who prefer working from the terminal. 

## tldr 
 
> Command-line tool to interact with Google Drive.
> Folder/file ID can be obtained from the Google Drive folder or ID URL.
> More information: <https://github.com/gdrive-org/gdrive>.

- Upload a local path to the parent folder with the specified ID:

`gdrive upload -p {{id}} {{path/to/file_or_folder}}`

- Download file or directory by ID to current directory:

`gdrive download {{id}}`

- Download to a given local path by its ID:

`gdrive download --path {{path/to/folder}} {{id}}`

- Create a new revision of an ID using a given file or folder:

`gdrive update {{id}} {{path/to/file_or_folder}}`
