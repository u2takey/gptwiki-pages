# stegsnow 
## chatgpt 
Stegsnow is a command-line tool that is used to hide secret messages in ASCII text files by appending white spaces or tabs to each character in the message. The resulting file looks and behaves like the original text file and can be transmitted as such without arousing suspicion.

Here are some of the basic options and usage of stegsnow:

1. To encode a secret message into a text file, you can run the following command:

    `$ stegsnow -C -p password < input.txt > output.txt`

    In this command, the `-C` option tells stegsnow to encode the message, `-p` is used to specify a password (which you will need to know to decode the message), `< input.txt` specifies the input file, and `> output.txt` specifies the output file.

2. To decode a message from a stegsnow-encoded file, you can use the following command:

    `$ stegsnow -C -p password < encoded.txt`

    Here, the `-C` option tells stegsnow to decode the message, `-p` specifies the password, and `< encoded.txt` specifies the encoded file.

3. Other options that can be used with stegsnow include:

    - `-f`: force stegsnow to encode or decode the message even if it is not password-protected.
    
    - `-S`: handle spaces in the message (default behavior is to ignore spaces).
    
    - `-T`: handle tabs in the message (default behavior is to ignore tabs).
    
    - `-s`: specify the size of the steganographic key (default is 8 bits).

    - `-V`: print the version number.

    - `-h`: print help information. 

## tldr 
 
> Steganography tool for concealing and extracting messages in text files encoded as tabs and spaces.
> More information: <https://darkside.com.au/snow/manual.html>.

- Extract [m]essage from file:

`stegsnow {{path/to/file.txt}}`

- Extract [C]ompressed and [p]assword protected [m]essage from file:

`stegsnow -C -p {{password}} {{path/to/file.txt}}`

- Determine approximate [S]torage capacity with line [l]ength less than 72 for file:

`stegsnow -S -l 72 {{path/to/file.txt}}`

- Conceal [m]essage in text from file and save to result:

`stegsnow -m '{{message}}' {{path/to/file.txt}} {{path/to/result.txt}}`

- Conceal message [f]ile content [C]ompressed in text from file and save to result:

`stegsnow -C -f '{{path/to/message.txt}}' {{path/to/file.txt}} {{path/to/result.txt}}`

- Conceal [m]essage [C]ompressed and [p]assword protected in text from file and save to result:

`stegsnow -C -p {{password}} -m '{{message}}' {{path/to/file.txt}} {{path/to/result.txt}}`
