# nkf 
## chatgpt 
The "nkf" command stands for "Network Kanji Filter". It is an open-source tool developed in Japan for converting Japanese text between various character encodings, such as EUC-JP, Shift_JIS, UTF-8, and ISO-2022-JP.

The nkf command is used to perform encoding conversions on character data. It is primarily used for converting Japanese text between the various character encodings. It can also perform other transformations, such as newline conversion or character set detection.

The nkf command can be run in a terminal with various options and arguments. Some of the most commonly used options include the following:

- "-w" (wide output): This option converts the input text to UTF-8 encoding.
- "-s" (assume Shift_JIS input): This option forces the input encoding to be Shift_JIS.
- "-e" (assume EUC-JP input): This option forces the input encoding to be EUC-JP.
- "-j" (assume ISO-2022-JP input): This option forces the input encoding to be ISO-2022-JP.
- "-Lw" (guess input encoding and convert to wide output): This option tries to detect the input encoding and convert it to UTF-8.

Overall, the nkf command is a useful tool for working with Japanese text and performing encoding conversions. 

## tldr 
 
> Network kanji filter.
> Converts kanji code from one encoding to another.
> More information: <https://manned.org/nkf>.

- Convert to UTF-8 encoding:

`nkf -w {{path/to/file.txt}}`

- Convert to SHIFT_JIS encoding:

`nkf -s {{path/to/file.txt}}`

- Convert to UTF-8 encoding and overwrite the file:

`nkf -w --overwrite {{path/to/file.txt}}`

- Set new line code to LF and overwrite (UNIX type):

`nkf -d --overwrite {{path/to/file.txt}}`

- Set new line code to CRLF and overwrite (windows type):

`nkf -c --overwrite {{path/to/file.txt}}`

- Decrypt mime file and overwrite:

`nkf -m --overwrite {{path/to/file.txt}}`
