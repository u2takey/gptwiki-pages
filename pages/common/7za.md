# 7za 
## chatgpt 
7za is a command-line file archiving utility that allows users to compress and extract files from archives on various operating systems, including Windows, Linux, and macOS.

Here's a breakdown of the command and its usage:

7za [options] [<commands>]

The command is made up of two parts - options and commands.

- Options: These are additional settings or parameters that modify the behavior of the command. Some commonly used options in 7za include:

  -a : Set archive type (e.g., "-a zip" for creating a Zip archive).
  
  -m : Set compression method (e.g., "-m0=PPMd" for using the PPMd compression method).
  
  -p : Set password for archives that require it.
  
  -t : Set archive type (e.g., "-tzip" for creating a Zip archive).
  
  -x : Exclude files from the archive.
  
  -y : Assume "Yes" to prompts (e.g., when extracting files).

- Commands: This is the action that 7za will perform on the archive file. Some commonly used commands include:

  a : Add files to an archive.
  
  e : Extract files from an archive.
  
  l : List contents of an archive.
  
  x : Extract files from an archive with full paths.

For example, to create a Zip archive of all files in the current directory and its subdirectories, you can use the following command:

7za a -tzip -r myarchive.zip *

Here, "a" is the command to add files to an archive, "-tzip" is the option to specify the archive type as Zip, "-r" is the option to include files in subdirectories, and "*" is the argument to include all files in the current directory. The resulting archive will be named "myarchive.zip".

Overall, 7za is a powerful command-line tool for managing archives, compressing and extracting files, and applying various settings and options to customize the process. 

## tldr 
 
> File archiver with a high compression ratio.
> Similar to `7z` except that it supports fewer file types but is cross-platform.
> More information: <https://www.7-zip.org>.

- [a]rchive a file or directory:

`7za a {{path/to/archive.7z}} {{path/to/file_or_directory}}`

- Encrypt an existing archive (including file names):

`7za a {{path/to/encrypted.7z}} -p{{password}} -mhe={{on}} {{path/to/archive.7z}}`

- E[x]tract an archive preserving the original directory structure:

`7za x {{path/to/archive.7z}}`

- E[x]tract an archive to a specific directory:

`7za x {{path/to/archive.7z}} -o{{path/to/output}}`

- E[x]tract an archive to `stdout`:

`7za x {{path/to/archive.7z}} -so`

- [a]rchive using a specific archive type:

`7za a -t{{7z|bzip2|gzip|lzip|tar|...}} {{path/to/archive.7z}} {{path/to/file_or_directory}}`

- [l]ist the contents of an archive:

`7za l {{path/to/archive.7z}}`

- List available archive types:

`7za i`
