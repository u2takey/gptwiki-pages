# xdg-mime 
## chatgpt 
xdg-mime is a command-line tool that is used to query or set file type associations in a desktop environment that adheres to the freedesktop.org standards. Here's a breakdown of the possible options and arguments that can be used with this command:

Usage: `xdg-mime [options] command [filetype|desktop_file] [command_options]`

Options:
- `-h/--help`: Print help message.
- `-q/--query`: Query current default applications for given file type or desktop file.
- `-m/--mime`: Only show MIME types that are handled by the specified desktop environment.
- `-n/--novendor`: List the MIME types without their corresponding 'vendor' prefix (e.g. 'application/x-tar' instead of 'application/x-gnu-tar').
- `-a/--add`: Add a new MIME type mapping.
- `-r/--remove`: Remove an existing MIME type mapping.
- `--update-icon-cache`: Update the desktop icon theme caches after changing MIME icons.

Commands:
- `default`: Query or set the default application for a given MIME type or desktop file.
- `query`: Query the MIME type for a given file name.
- `guess`: Guess the MIME type for a given file name.
- `mimeinfo`: Show information about a MIME type.
- `mimetype`: Show the MIME type for a file.

Filetype argument:
- If a filetype string is provided (e.g. 'text/plain'), the command will show or change the default application for that file type.
- If a desktop file name is provided (e.g. 'gedit.desktop'), the command will show or change the default application associated with that desktop file.

Command options:
- Depending on the chosen command, additional options can be provided to set or query various properties related to file type associations.

Overall, xdg-mime is a versatile tool for managing file type associations in a desktop environment (e.g. setting a default text editor for .txt files). 

## tldr 
 
> Query and manage MIME types according to the XDG standard.
> More information: <https://portland.freedesktop.org/doc/xdg-mime.html>.

- Display the MIME type of a file:

`xdg-mime query filetype {{path/to/file}}`

- Display the default application for opening PNGs:

`xdg-mime query default {{image/png}}`

- Display the default application for opening a specific file:

`xdg-mime query default $(xdg-mime query filetype {{path/to/file}})`

- Set imv as the default application for opening PNG and JPEG images:

`xdg-mime default {{imv.desktop}} {{image/png}} {{image/jpeg}}`
