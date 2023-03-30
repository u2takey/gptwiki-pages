# zenity 
## chatgpt 
Zenity is a command-line tool that helps to generate graphical user interface dialogs and forms for shell and bash scripts. It is commonly used to create simple GUI dialogs like input boxes, progress bars, file selection dialogs, etc.

The syntax for the Zenity command is listed below:

zenity [option]…

Here, the “option” refers to the various command-line switches or flags that can be used with the Zenity command to customize its behavior and appearance.

Some examples of the options used with Zenity command are:

--entry: This option is used to create a simple input dialog box in which the user can enter a single line of text.

--file-selection: This option is used to create a file selection dialog box where the user can browse and select a file from the system.

--info: This option is used to create a dialog box that provides information to the user, usually in the form of an informative text message.

--question: This option is used to create a dialog box that asks the user a yes/no question, and the user can respond by either clicking on the “yes” or “no” button.

--progress: This option helps to create a dialog box with a progress bar that displays the progress of a long-running task.

By using these and other Zenity options with customized text labels and buttons, developers can easily create interactive dialogs and forms that run in a terminal window, without the need for heavy-weight graphical toolkits or programming frameworks. 

## tldr 
 
> Display dialogs from the command-line/shell scripts.
> Return user-inserted values or 1 if error.
> More information: <https://manned.org/zenity>.

- Display the default question dialog:

`zenity --question`

- Display an info dialog displaying the text "Hello!":

`zenity --info --text="{{Hello!}}"`

- Display a name/password form and output the data separated by ";":

`zenity --forms --add-entry="{{Name}}" --add-password="{{Password}}" --separator="{{;}}"`

- Display a file selection form in which the user can only select directories:

`zenity --file-selection --directory`

- Display a progress bar which updates its message every second and show a progress percent:

`{{(echo "#1"; sleep 1; echo "50"; echo "#2"; sleep 1; echo "100")}} | zenity --progress`
