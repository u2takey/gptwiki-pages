# whiptail 
## chatgpt 
`whiptail` is a command-line interface (CLI) tool for creating dialog boxes in Unix and Unix-like operating systems. It is commonly used in shell scripts to provide interactive prompts and menus for users.

The most basic syntax for invoking `whiptail` is:

```
whiptail [options] [text height width]
```

The `options` parameter can be used to specify various options such as the type of dialog box to display (e.g., message, input, checklist, radiolist, menu, etc.), button labels, default values, etc.

The `text` parameter is used to specify the message or prompt to display in the dialog box. If this parameter is omitted, `whiptail` will read the message from standard input.

The `height` and `width` parameters are used to specify the dimensions of the dialog box in characters. These parameters are optional, and the default values are usually sufficient for most use cases.

Here are a few examples of how `whiptail` can be used:

```
# display a simple message box
whiptail --msgbox "Hello World!" 8 20

# display an input box and capture user input
input=$(whiptail --inputbox "Enter your name:" 8 40 John --title "User Information" 3>&1 1>&2 2>&3)

# display a checklist and capture user selections
options=(1 "Option 1" off
         2 "Option 2" off
         3 "Option 3" on)
choices=$(whiptail --checklist "Choose options:" 12 60 3 "${options[@]}" 3>&1 1>&2 2>&3)
```

In the first example, `whiptail` displays a simple message box with the message "Hello World!".

In the second example, `whiptail` displays an input box with the message "Enter your name:", a default value of "John", and a title of "User Information". The `3>&1 1>&2 2>&3` syntax is used to redirect standard output (which `whiptail` uses for user input) to file descriptor 3, and redirect standard error (which `whiptail` uses for output) to file descriptor 2. This allows the user input to be captured and stored in the `input` variable.

In the third example, `whiptail` displays a checklist with three options ("Option 1", "Option 2", and "Option 3") and captures the user's selections in the `choices` variable. The `options` array specifies each option as an array of three elements: the option index (1-3), the option text, and the initial selection state (on or off). The `3>&1 1>&2 2>&3` syntax is used again to capture user input and output. 

## tldr 
 
> Display text-based dialog boxes from shell scripts.
> More information: <https://manned.org/whiptail>.

- Display a simple message:

`whiptail --title "{{title}}" --msgbox "{{message}}" {{height_in_chars}} {{width_in_chars}}`

- Display a boolean choice, returning the result through the exit code:

`whiptail --title "{{title}}" --yesno "{{message}}" {{height_in_chars}} {{width_in_chars}}`

- Customise the text on the yes / no buttons:

`whiptail --title "{{title}}" --yes-button "{{text}}" --no-button "{{text}}" --yesno "{{message}}" {{height_in_chars}} {{width_in_chars}}`

- Display a text input box:

`{{result_variable_name}}="$(whiptail --title "{{title}}" --inputbox "{{message}}" {{height_in_chars}} {{width_in_chars}} {{default_text}} 3>&1 1>&2 2>&3)"`

- Display a password input box:

`{{result_variable_name}}="$(whiptail --title "{{title}}" --passwordbox "{{message}}" {{height_in_chars}} {{width_in_chars}} 3>&1 1>&2 2>&3)"`

- Display a multiple-choice menu:

`{{result_variable_name}}=$(whiptail --title "{{title}}" --menu "{{message}}" {{height_in_chars}} {{width_in_chars}} {{menu_display_height}} "{{value_1}}" "{{display_text_1}}" "{{value_n}}" "{{display_text_n}}" ..... 3>&1 1>&2 2>&3)`
