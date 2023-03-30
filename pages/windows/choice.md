# choice 
## chatgpt 
The "choice" command is a Windows command that prompts the user to select a number from a predefined list of options, and then performs an action based on the user's selection.

The syntax of the "choice" command is as follows:

    choice /C:options /N /T:timeout /D:default /M:message

Where:
- /C:options specifies a list of characters that corresponds to the available options. The options must be enclosed in double quotes and separated by commas.
- /N specifies that the selected option should be displayed as a simple number instead of a character.
- /T:timeout specifies the number of seconds before the default option (if defined) is selected automatically.
- /D:default specifies the default option to be selected if the user does not provide a valid input within the specified timeout period.
- /M:message specifies the message to be displayed to the user, which includes the available options.

For example, the following command prompts the user to select an option from the list of "Y" and "N", and then performs a specific action based on the selection:
```
choice /C:YN /N /M:"Do you want to continue? Press Y for YES and N for NO."
if errorlevel 2 (
    echo You selected NO.
) else (
    echo You selected YES.
)
```

In this example, the /C:YN option specifies the available options, /N specifies that the selected option should be displayed as a number (1 for Y, 2 for N), and /M specifies the message to be displayed to the user. The "if" statement checks the errorlevel value returned by the "choice" command, which corresponds to the selected option. If the value is 2, it means the user selected "N", so the "You selected NO" message is displayed. If the value is not 2 (i.e., the user selected "Y" or did not provide a valid input within the specified timeout), the "You selected YES" message is displayed. 

## tldr 
 
> Prompt user to select a choice and return the selected choice index.
> More information: <https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/choice>.

- Prompt the current user to select a `Y` or `N` choice:

`choice`

- Prompt the current user to select a [c]hoice from a specific set:

`choice /c {{AB}}`

- Prompt the current user to select a choice with a specific [m]essage:

`choice /m "{{message}}"`

- Prompt the current user to select a [c]ase-[s]ensitive [c]hoice from a specific set:

`choice /cs /c {{Ab}}`

- Prompt the current user to select a choice and prefer the [d]efault choice in a specific [t]ime:

`choice /t {{5}} /d {{N}}`

- Display help:

`choice /?`
