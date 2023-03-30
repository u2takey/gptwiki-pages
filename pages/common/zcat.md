# zcat 
## chatgpt 
zcat is a Unix command that is used to display the contents of a compressed file on the terminal without actually decompressing it.

The command works by first reading the compressed file and then decompressing it in real-time before displaying its contents on the terminal. This helps save disk space by avoiding the need to first decompress the file before viewing its contents, especially with large files.

Here is the general syntax of the zcat command:

zcat [compressed_file]

Here, [compressed_file] refers to the name of the compressed file that you want to view. The file can be compressed in the gzip (.gz) or the bzip2 (.bz2) format.

To use the zcat command, simply type zcat followed by the name of the compressed file and press enter. The contents of the file will be displayed on the terminal.

For example, if you want to view the contents of a file named example.txt.gz, you would use the following command:

zcat example.txt.gz

This will display the contents of the example.txt file on the terminal, without actually decompressing it. 

## tldr 
 
> Print data from gzip compressed files.
> More information: <https://www.gnu.org/software/gzip/manual/gzip.html>.

- Print the uncompressed contents of a gzipped file to the standard output:

`zcat {{file.txt.gz}}`

- Print compression details of a gzipped file to the standard output:

`zcat -l {{file.txt.gz}}`
