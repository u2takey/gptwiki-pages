# yank 
## chatgpt 
The "yank" command is a text manipulation tool used to copy text to the clipboard or buffer in the Vi and Vim text editors.

In Vim, the "yank" command is abbreviated as "y". To use the yank command, first, position the cursor at the beginning of the text you want to copy. Then enter the command mode by pressing the "Escape" key. Once in command mode, type the letter "y" followed by a movement command that selects the text you want to copy.

For example, to copy the current line, type "yy". To copy four lines, type "4yy".

After copying the text with the "yank" command, it can be pasted elsewhere in the document using the "p" command. The "p" command will paste the copied text after the current cursor position.

In summary, the "yank" command in Vim is a useful text manipulation tool for copying text to the clipboard or buffer, which can then be pasted elsewhere in the document. 

## tldr 
 
> Read input from `stdin` and display a selection interface that allows a field to be selected and copied to the clipboard.
> More information: <https://manned.org/yank>.

- Yank using the default delimiters (\f, \n, \r, \s, \t):

`{{sudo dmesg}} | yank`

- Yank an entire line:

`{{sudo dmesg}} | yank -l`

- Yank using a specific delimiter:

`{{echo hello=world}} | yank -d {{=}}`

- Only yank fields matching a specific pattern:

`{{ps ux}} | yank -g "{{[0-9]+}}"`
