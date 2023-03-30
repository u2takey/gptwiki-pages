# photorec 
## chatgpt 
Photorec is a command line program designed to recover lost files from various storages media such as hard disks, CDs, USB pen drives, and memory cards.

When executed, Photorec reads the source storage media block by block and searches for deleted or lost file signatures by analyzing data. Once it discovers file signatures, it extracts and saves them to a specified destination folder, typically external media to avoid overwriting existing data on the target media.

Photorec supports thousands of file formats, including popular photo, video, audio, and document formats. It can recover files even from damaged or corrupted file systems, making it an indispensable tool for data recovery specialists and professionals.

Photorec has a user-friendly interface with easy-to-understand prompts that guide you through the recovery process. However, advanced users can use command-line options to customize the recovery process and have more control over the recovery process.

Overall, Photorec is a reliable and efficient tool for restoring lost or deleted files, and its support for multiple platforms makes it a valuable asset for anyone dealing with data recovery. 

## tldr 
 
> Deleted file recovery tool.
> It is recommended to write recovered files to a disk separate to the one being recovered from.
> More information: <https://www.cgsecurity.org/wiki/PhotoRec>.

- Run PhotoRec on a specific device:

`sudo photorec {{/dev/sdb}}`

- Run PhotoRec on a disk image (`image.dd`):

`sudo photorec {{path/to/image.dd}}`
