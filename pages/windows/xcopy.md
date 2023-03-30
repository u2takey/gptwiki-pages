# xcopy 
## chatgpt 
The xcopy command is a Windows file utility used to copy files and directories from one location to another. Here is a detailed explanation of the xcopy command:

Syntax:
xcopy source [destination] [/A | /M] [/D[:date]] [/P] [/H] [/K] [/R] [/S] [/E] [/T] [/U] [/G] [/Y] [/C] [/I] [/Q] [/N] [/O] [/X] [/L] [/V] [/F] [/B] [/W] [/J] [/Z] [/EXCLUDE:file] 

Parameters:

- source: Specifies the path and name of the file or files to copy.
- destination: Specifies the path and name of the destination directory. If you omit destination, xcopy copies the files to the current directory.
- /A: Copies only files that have the archive attribute set, and turns off the archive attribute.
- /M: Copies only files that have the archive attribute set, and does not turn off the archive attribute.
- /D: Specifies the date before or on which files were last modified. If you do not specify a date, xcopy copies only those files whose source time is newer than the destination time.
- /P: Prompts you to confirm whether you want to create each destination file.
- /H: Copies hidden files and folders.
- /K: Copies attributes, including read-only, hidden, and system files, to the destination files.
- /R: Copies read-only files.
- /S: Copies subdirectories and files.
- /E: Copies subdirectories, including empty ones, and files.
- /T: Creates directory structure, but does not copy files. Used to make a new directory with the same subdirectory structure as an existing directory.
- /U: Copies only files that already exist in destination.
- /G: Copies encrypted files in EFS partitions.
- /Y: Suppresses prompts that ask you to confirm that you want to overwrite existing files.
- /C: Continues copying even if errors occur.
- /I: Creates destination directory if it does not already exist.
- /Q: Does not display message during copying process (quiet mode).
- /N: Creates a copy but does not use short filenames.
- /O: Copies file ownership and ACL information.
- /X: Copies file audit settings.
- /L: Lists files that would be copied, without actually copying them.
- /V: Verifies each file that is copied.
- /F: Displays full source and destination for each file being copied.
- /B: Copies files in binary mode (useful for copying non-text files).
- /W: Waits for a key press before copying the next file.
- /J: Copies files without buffering.
- /Z: Copies files in restartable mode, allowing the copy operation to resume from the point of failure.
- /EXCLUDE:file: Specifies a list of files or directories to exclude from the copy.

The xcopy command is a powerful tool for copying files and directories in Windows. With the ability to specify a wide range of options, it can be used in a variety of situations, from simple one-time file copy operations to complex backup and synchronization tasks. 

## tldr 
 
> Copy files and directory trees.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/xcopy>.

- Copy the file(s) to the specified destination:

`xcopy {{path\to\file_or_directory}} {{path\to\destination_directory}}`

- List files that will be copied before copying:

`xcopy {{path\to\file_or_directory}} {{path\to\destination_directory}} /p`

- Copy the directory structure only, excluding files:

`xcopy {{path\to\file_or_directory}} {{path\to\destination_directory}} /t`

- Include empty directories when copying:

`xcopy {{path\to\file_or_directory}} {{path\to\destination_directory}} /e`

- Keep the source ACL in the destination:

`xcopy {{path\to\file_or_directory}} {{path\to\destination_directory}} /o`

- Allow resuming when network connection is lost:

`xcopy {{path\to\file_or_directory}} {{path\to\destination_directory}} /z`

- Disable the prompt when the file exists in the destination:

`xcopy {{path\to\file_or_directory}} {{path\to\destination_directory}} /y`

- Display detailed usage information:

`xcopy /?`
