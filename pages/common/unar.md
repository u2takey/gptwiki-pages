# unar 
## chatgpt 
The command "unar" is a utility program used to extract archives in various formats such as ZIP, RAR, 7-zip, tar, and many more. The unar command is applicable for Mac OS X and Linux operating systems. 

When you execute the "unar" command, the utility program will prompt you to provide the path to the archive file that you want to extract. Once you have provided the path, the utility program will analyze and extract the archive file contents to the desired location.

Some of the options that can be used with the "unar" command are:

- "-q" or "--quiet": This option enables the utility program to run in silent mode without displaying any prompts or progress messages on the console.

- "-f" or "--force": This option enables the utility program to override any existing files during the extraction process without prompting the user.

- "-o" or "--output-directory" [directory]: This option sets the output directory for the extracted files.

- "-v" or "--verbose": This option enables the utility program to display more details about the extraction process.

Overall, the "unar" command is a useful utility program for extracting various archive formats in Mac and Linux operating systems. 

## tldr 
 
> Extract contents from archive files.
> More information: <https://manned.org/unar>.

- Extract an archive to the current directory:

`unar {{archive}}`

- Extract an archive to the specified directory:

`unar -o {{path/to/directory}} {{archive}}`

- Force overwrite if files to be unpacked already exist:

`unar -f {{archive}}`

- Force rename if files to be unpacked already exist:

`unar -r {{archive}}`

- Force skip if files to be unpacked already exist:

`unar -s {{archive}}`
