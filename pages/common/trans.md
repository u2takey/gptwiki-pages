# trans 
## chatgpt 
The "trans" command stands for "transmission" and is used to transfer files between two systems over a network. It is usually used to move files from one computer to another.

Some common options that can be used with the "trans" command are:

- "-r": This option is used to recursively transfer entire directories and their contents.
- "-u": This option is used to update files that already exist on the destination system. If a file on the destination system has a more recent timestamp than the file being transferred, then the transfer will be skipped.
- "-v": This option is used to enable verbose output, which displays more detailed information about the transfer process.
- "-z": This option is used to compress files during transfer, which can make the transfer faster and more efficient.

To use the "trans" command, you need to specify the source and destination systems, as well as the files or directories that you want to transfer. For example, to transfer a file named "file.txt" from a local system to a remote system with the IP address "192.168.1.100", you could use the following command:

trans file.txt 192.168.1.100:/path/to/destination

This command would copy "file.txt" to the "/path/to/destination" directory on the remote system. If you wanted to transfer an entire directory and its contents, you could use the "-r" option, like this:

trans -r /path/to/source 192.168.1.100:/path/to/destination

This command would copy the entire "/path/to/source" directory to the "/path/to/destination" directory on the remote system. 

## tldr 
 
> Translate Shell is a command-line translator.
> More information: <https://github.com/soimort/translate-shell>.

- Translate a word (language is detected automatically):

`trans "{{word_or_sentence_to_translate}}"`

- Get a brief translation:

`trans --brief "{{word_or_sentence_to_translate}}"`

- Translate a word into french:

`trans :{{fr}} {{word}}`

- Translate a word from German to English:

`trans {{de}}:{{en}} {{Schmetterling}}`

- Behave like a dictionary to get the meaning of a word:

`trans -d {{word}}`
