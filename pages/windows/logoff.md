# logoff 
## chatgpt 
The "logoff" command is a Windows command used to log off the current user from the system. When executed, it logs you off your current session and returns you to the login screen. This means that all unsaved work and open applications running under the current session will be closed, and you will be required to re-enter your user credentials to use the system again. 

In addition to logging off, there are other ways of ending a user session, including shutting down or restarting the computer. However, the "logoff" command is preferred when you want to sign out of your user account but want to keep the system running for someone else to use. 

The command can be executed in several ways: 

1. Using the Start menu: Click the Start button, select the Power icon, and select "Log off."
2. Using the command prompt: Open the command prompt and type "logoff" and press enter. 
3. Using the Run dialog box: Press the Windows key + R to open the Run dialog box. Type "logoff" and press enter.

Overall, the "logoff" command provides an easy and quick way to log out of a Windows session and keep the system running for other users without fully shutting down the computer. 

## tldr 
 
> Terminate a login session.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/logoff>.

- Terminate the current session:

`logoff`

- Terminate a session by its name or id:

`logoff {{session_name|session_id}}`

- Terminate a session on a specific server connected through RDP:

`logoff {{session_name|session_id}} /server:{{servername}}`
