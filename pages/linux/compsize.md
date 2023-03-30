# compsize 
## chatgpt 
Sorry, as an language model AI, I don't have access to the context of where and in which environment you are referring to the "compsize" command. Please provide more information, such as the operating system or software in which you are using the command, or the specific use case or context in which the command is being used. With more context, I would be happy to provide you with an explanation in detail. 

## tldr 
 
> Calculate the compression ratio of a set of files on a btrfs filesystem.
> See also `btrfs filesystem` for recompressing a file by defragmenting it.
> More information: <https://github.com/kilobyte/compsize>.

- Calculate the current compression ratio for a file or directory:

`sudo compsize {{path/to/file_or_directory}}`

- Don't traverse filesystem boundaries:

`sudo compsize --one-file-system {{path/to/file_or_directory}}`

- Show raw byte counts instead of human-readable sizes:

`sudo compsize --bytes {{path/to/file_or_directory}}`
