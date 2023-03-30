# copyq 
## chatgpt 
As an AI language model, I am not sure which platform or operating system you are referring to. However, in general, the "copyq" command is a utility tool used to create a list of copied items and organize them for easy access. It is typically used on Linux systems.

The "copyq" command is used to monitor the clipboard activity and record any data that is copied. It is particularly useful when there is a need to copy multiple items and paste them one after another.

When the "copyq" command is used, it will start monitoring the clipboard in the background. Any data that is copied will be added to a list of items that can be accessed later. The copied items can be organized into different categories and labeled for easy reference.

Additionally, the "copyq" command can be used to perform various other tasks, such as removing duplicate items, creating shortcuts, and executing scripts.

Overall, the "copyq" command is a powerful and convenient tool for managing clipboard data on Linux systems. 

## tldr 
 
> Clipboard manager with advanced features.
> More information: <https://hluk.github.io/CopyQ/>.

- Launch CopyQ to store clipboard history:

`copyq`

- Show current clipboard content:

`copyq clipboard`

- Insert raw text into the clipboard history:

`copyq add -- {{text1}} {{text2}} {{text3}}`

- Insert text containing escape sequences ('\n', '\t') into the clipboard history:

`copyq add {{firstline\nsecondline}}`

- Print the content of the first 3 items in the clipboard history:

`copyq read 0 1 2`

- Copy a file's contents into the clipboard:

`copyq copy < {{file.txt}}`

- Copy a JPEG image into the clipboard:

`copyq copy image/jpeg < {{image.jpg}}`
