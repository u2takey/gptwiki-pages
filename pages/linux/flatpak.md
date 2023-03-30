# flatpak 
## chatgpt 
Flatpak is a command-line tool that is used to manage, install, and run sandboxed applications or software packages in Linux operating systems. It uses a centralized repository to store and distribute applications, and it provides a secure environment for running applications using runtime and platform libraries. 

The flatpak command offers a variety of functions and options to manage applications on your system. Here are some of the most commonly used ones:

- flatpak install: This command is used to install a flatpak application from a remote repository by specifying the name of the application or the URL of the remote repository.

- flatpak update: This command is used to update all installed flatpak applications to the latest version available on the remote repository.

- flatpak uninstall: This command is used to remove a flatpak application from your system.

- flatpak run: This command is used to run a flatpak application.

- flatpak list: This command is used to list all the flatpak applications that are installed on your system.

- flatpak info: This command is used to get detailed information about a specific flatpak application.

- flatpak search: This command is used to search for available flatpak applications on the remote repository.

- flatpak remote-add: This command is used to add a new remote flatpak repository to your system.

Overall, the flatpak command provides an efficient way to manage applications in Linux systems, with a focus on security and portability. 

## tldr 
 
> Build, install and run flatpak applications and runtimes.
> More information: <https://docs.flatpak.org/en/latest/flatpak-command-reference.html#flatpak>.

- Run an installed application:

`flatpak run {{name}}`

- Install an application from a remote source:

`flatpak install {{remote}} {{name}}`

- List all installed applications and runtimes:

`flatpak list`

- Update all installed applications and runtimes:

`flatpak update`

- Add a remote source:

`flatpak remote-add --if-not-exists {{remote_name}} {{remote_url}}`

- Remove an installed application:

`flatpak remove {{name}}`

- Remove all unused applications:

`flatpak remove --unused`

- Show information about an installed application:

`flatpak info {{name}}`
