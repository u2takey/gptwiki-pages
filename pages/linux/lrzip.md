# lrzip 
## chatgpt 
lrzip is a command-line tool used for compressing and decompressing files. It is designed to provide high compression ratios while maintaining very fast decompression speeds. The following is a detailed explanation of the lrzip command:

1. Installation
  To use the lrzip command, you first need to install the tool on your system. This can typically be done using the package manager for your operating system, such as apt or yum.

2. Usage
  The basic syntax for lrzip is as follows:

  lrzip [options] input_file
  
  This will compress the specified input file using the default settings and output the compressed file to the same location with the ".lrz" extension appended. 

3. Compression levels
  lrzip supports several compression levels, which can be specified using the "-L" option followed by a number from 0 to 9. The higher the number, the greater the compression ratio, but also the longer the compression time.

4. Encryption
  lrzip supports encryption of compressed files using the "-e" option followed by a passphrase. This passphrase is used to encrypt and decrypt the file. 

5. Decompression
  To decompress a compressed lrzip file, simply specify the compressed file as the input to the lrzip command, and use the "-d" option to indicate that you want to decompress the file instead of compressing it.

6. Additional options
  There are several other options available for the lrzip command, which can be viewed by running "man lrzip" or "lrzip --help". 

Overall, lrzip is a powerful and flexible command-line tool for compressing and decompressing files with high compression ratios and fast decompression speeds. 

## tldr 
 
> A large file compression program.
> See also `lrunzip`, `lrztar`, `lrzuntar`.
> More information: <https://manned.org/lrzip>.

- Compress a file with LZMA - slow compression, fast decompression:

`lrzip {{filename}}`

- Compress a file with BZIP2 - good middle ground for compression/speed:

`lrzip -b {{filename}}`

- Compress with ZPAQ - extreme compression, but very slow:

`lrzip -z {{filename}}`

- Compress with LZO - light compression, extremely fast decompression:

`lrzip -l {{filename}}`

- Compress a file and password protect/encrypt it:

`lrzip -e {{filename}}`

- Override the number of processor threads to use:

`lrzip -p {{8}} {{filename}}`
