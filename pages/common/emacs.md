# emacs 
## chatgpt 
Emacs is a popular text editor used by programmers and other users to write and edit text files. It is an open-source software and can be installed on various operating systems such as Linux, Windows, and macOS.

When the command "emacs" is entered into the terminal, the Emacs editor is launched, and the user can start creating and editing text files. 

Once the Emacs editor is launched, the user can create a new file by pressing the "Ctrl+X Ctrl+F" keys. This will prompt the user to enter the file name and create a new file with that name in the current directory.

The user can then start editing the file by typing the text. Emacs allows for various customization options, such as changing the font size, color, and syntax highlighting.

Emacs also has various keyboard shortcuts that can be used to perform different operations, such as saving the file ("Ctrl+X Ctrl+S"), cutting and pasting text, and searching for text.

When the user is done editing the file, they can save and close the file by pressing "Ctrl+X Ctrl+S" and then "Ctrl+X Ctrl+C". This will save the file and exit the Emacs editor session.

Overall, the Emacs command is a powerful tool for creating and editing text files and can be customized to suit the user's needs. 

## tldr 
 
> The extensible, customizable, self-documenting, real-time display editor.
> See also `emacsclient`.
> More information: <https://www.gnu.org/software/emacs>.

- Start Emacs and open a file:

`emacs {{path/to/file}}`

- Open a file at a specified line number:

`emacs +{{line_number}} {{path/to/file}}`

- Run an Emacs Lisp file as a script:

`emacs --script {{path/to/file.el}}`

- Start Emacs in console mode (without an X window):

`emacs --no-window-system`

- Start an Emacs server in the background (accessible via `emacsclient`):

`emacs --daemon`

- Stop a running Emacs server and all its instances, asking for confirmation on unsaved files:

`emacsclient --eval '(save-buffers-kill-emacs)'`

- Save a file in Emacs:

`Ctrl + X, Ctrl + S`

- Quit Emacs:

`Ctrl + X, Ctrl + C`
