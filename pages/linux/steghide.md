# steghide 
## chatgpt 
Steghide is a command-line tool used for hiding data in various types of digital media files (such as image, audio, and video files). The tool uses a technique called steganography to embed data within the media files in such a way that it is not noticeable to the human eye.

The steghide command can be used to both hide and extract data from digital media files. Its basic syntax is as follows:

steghide <command> [options]

Where "<command>" represents the specific action you want to perform (such as "embed" to hide data or "extract" to retrieve it), and "[options]" are any additional parameters or settings needed to complete the command.

To embed data into a media file using steghide, you would use the "embed" command and provide the path to the file you want to hide, as well as the path to the media file in which you want to hide it, and a password to protect the hidden data. For example:

steghide embed -ef secret.txt -cf image.jpg -p mypassword

This command would embed the contents of "secret.txt" into the "image.jpg" file, using the password "mypassword" to protect the hidden data.

To extract hidden data from a media file using steghide, you would use the "extract" command and again provide the path to the media file and the password used to protect the hidden data. For example:

steghide extract -sf image.jpg -p mypassword

This command would extract any hidden data from the "image.jpg" file, using the password "mypassword" to access it.

Overall, steghide is a useful tool for securing sensitive data or communicating covertly, by hiding information within seemingly innocent digital media files. 

## tldr 
 
> Steganography tool for JPEG, BMP, WAV and AU file formats.
> More information: <https://github.com/StefanoDeVuono/steghide>.

- Embed data in a PNG, prompting for a passphrase:

`steghide embed --coverfile {{path/to/image.png}} --embedfile {{path/to/data.txt}}`

- Extract data from a WAV audio file:

`steghide extract --stegofile {{path/to/sound.wav}}`

- Display file information, trying to detect an embedded file:

`steghide info {{path/to/file.jpg}}`

- Embed data in a JPEG image, using maximum compression:

`steghide embed --coverfile {{path/to/image.jpg}} --embedfile {{path/to/data.txt}} --compress {{9}}`

- Get the list of supported encryption algorithms and modes:

`steghide encinfo`

- Embed encrypted data in a JPEG image, e.g. with Blowfish in CBC mode:

`steghide embed --coverfile {{path/to/image.jpg}} --embedfile {{path/to/data.txt}} --encryption {{blowfish|...}} {{cbc|...}}`
