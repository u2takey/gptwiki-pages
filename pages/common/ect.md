# ect 
## chatgpt 
I'm sorry, as an AI language model, I don't have enough context to know which specific "ect" command you are referring to. Please provide additional information or clarification about the command so I can give you a detailed explanation. 

## tldr 
 
> Efficient Compression Tool.
> File optimizer written in C++. It supports `.png`, `.jpg`, `.gzip` and `.zip` files.
> More information: <https://github.com/fhanau/Efficient-Compression-Tool>.

- Compress a file:

`ect {{path/to/file.png}}`

- Compress a file with specified compression level and multithreading (1=Fastest (Worst), 9=Slowest (Best), default is 3):

`ect -{{9}} --mt-deflate {{path/to/file.zip}}`

- Compress all files in a directory recursively:

`ect -recurse {{path/to/directory}}`

- Compress a file, keeping the original modification time:

`ect -keep {{path/to/file.png}}`

- Compress a file, stripping metadata:

`ect -strip {{path/to/file.png}}`
