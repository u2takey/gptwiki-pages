# Get-History 
## chatgpt 
The `Get-History` command is used in PowerShell to retrieve the command history of the current session. It allows you to see a list of all the commands that you've run in your current session, along with their IDs.

When you run `Get-History`, PowerShell will display a list of commands that you've executed in the terminal, with each command accompanied by a unique ID number. You can use these ID numbers to reference previous commands and perform various actions on them, such as repeating or editing them.

The `Get-History` command is particularly useful when you're working on a complex task and need to refer back to previous commands, or if you want to search for a particular command that you ran earlier but can't remember the exact details of.

Overall, `Get-History` is a very useful command for anyone working with PowerShell, as it helps streamline the workflow and make it easier to manage and keep track of past commands. 

## tldr 
 
> Display PowerShell command history.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.core/get-history>.

- Display the commands history list with ID:

`Get-History`

- Get PowerShell history item by ID:

`Get-History -Id {{id}}`

- Display the last N commands:

`Get-History -Count {{10}}`
