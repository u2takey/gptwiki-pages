# kdialog 
## chatgpt 
kdialog is a command-line utility provided by the KDE desktop environment, that displays graphical dialogs and user interfaces on the screen. It is typically used to prompt the user for some sort of input or confirmation, or to display messages or warnings.

Some of the common options and subcommands of kdialog are:

- --msgbox: Displays a simple message box with an OK button.
- --warningbox: Displays a warning message box with an OK button.
- --error: Displays an error message box with an OK button.
- --inputbox: Prompts the user for a string input, and returns the entered text.
- --password: Prompts the user for a password input, and returns the entered text. The input is masked for security reasons.
- --getsavefilename: Prompts the user to select a file name for saving, and returns the selected path.
- --getopenfilename: Prompts the user to select a file to open, and returns the selected path.
- --getexistingdirectory: Prompts the user to select an existing directory, and returns the selected path.
- --yesno: Displays a question dialog with Yes and No buttons, and returns 0 for Yes and 1 for No.

Overall, kdialog is a useful tool for developers and system administrators who need to create simple GUI applications or scripts with user interaction. Its versatility and ease of use make it a popular choice among KDE enthusiasts. 

## tldr 
 
> Show KDE dialog boxes from within shell scripts.
> More information: <https://develop.kde.org/deploy/kdialog/>.

- Open a dialog box displaying a specific message:

`kdialog --msgbox "{{message}}" "{{optional_detailed_message}}"`

- Open a question dialog with a `yes` and `no` button, returning `0` and `1`, respectively:

`kdialog --yesno "{{message}}"`

- Open a warning dialog with a `yes`, `no`, and `cancel` button, returning `0`, `1`, or `2` respectively:

`kdialog --warningyesnocancel "{{message}}"`

- Open an input dialog box and print the input to `stdout` when `OK` is pressed:

`kdialog --inputbox "{{message}}" "{{optional_default_text}}"`

- Open a dialog to prompt for a specific password and print it to `stdout`:

`kdialog --password "{{message}}"`

- Open a dialog containing a specific dropdown menu and print the selected item to `stdout`:

`kdialog --combobx "{{message}}" "{{item1}}" "{{item2}}" "{{...}}"`

- Open a file chooser dialog and print the selected file's path to `stdout`:

`kdialog --getopenfilename`

- Open a progressbar dialog and print a DBUS reference for communication to `stdout`:

`kdialog --progressbar "{{message}}"`
