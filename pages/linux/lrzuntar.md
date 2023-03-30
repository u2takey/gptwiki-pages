# lrzuntar 
## chatgpt 
As an AI language model, I am not aware of any command called "lrzuntar". However, both 'lz' and 'tar' are different commands that can be used in combination to compress/decompress tar archives with Lempel-Ziv (LZ) compression respectively.

The 'tar' command is used to create and extract tar archives, which are a collection of files packaged into a single file. The general syntax for creating an archive looks like this:

```tar -cvf archive.tar /path/to/directory```

Here, the -c flag tells tar to create a new archive, the -v flag enables verbose mode, and the -f flag specifies the name of the archive file. The last argument is the directory you want to archive.

The opposite of the -c flag, which is used to create new archives is -x flag which extracts the files from the archive back to the file system.

The 'lz' command is used to compress and decompress files using Lempel-Ziv (LZ) algorithms. The syntax for compressing a file looks like this:

```lz myfile.txt```

This creates a compressed file called 'myfile.txt.lz'. To decompress, simply run:

```unlz myfile.txt.lz```

This will restore the original file, 'myfile.txt'.

Combining both these commands to form "lrzuntar"could be to create or extract an archive that has compressed using LZ compression. 

## tldr 
 
> A wrapper for `lrunzip` to simplify decompression of directories.
> See also: `lrztar`, `lrzip`.
> More information: <https://manned.org/lrzuntar>.

- Decompress from a file to the current directory:

`lrzuntar {{path/to/archive.tar.lrz}}`

- Decompress from a file to the current directory using a specific number of processor threads:

`lrzuntar -p {{8}} {{path/to/archive.tar.lrz}}`

- Decompress from a file to the current directory and silently overwrite items that already exist:

`lrzuntar -f {{archive.tar.lrz}}`

- Specify the output path:

`lrzuntar -O {{path/to/directory}} {{archive.tar.lrz}}`

- Delete the compressed file after decompression:

`lrzuntar -D {{path/to/archive.tar.lrz}}`
