# protontricks 
## chatgpt 
The "protontricks" command is a utility tool associated with the Proton compatibility tool. Proton is a compatibility tool for Steam Play that enables Windows games to run on Linux operating systems. Protontricks provides a set of currently supported tricks that can be used for tweaking games that are running on Steam Play via Proton. 

The command is used to run these tricks over games or applications so that they can work optimally on a Linux system with the help of Proton. For example, some games may have performance issues owing to certain missing components or DLLs in a Linux environment. Protontricks can be used to install such additional components as required by a game to work as intended.

Overall, protontricks provides a handy collection of tools that can be used for installing different additional components, altering system settings or configurations to improve application compatibility, or troubleshooting in case an application is not running as intended. The command can be used to customize the Proton/Wine runtime before running a game or application, providing a smoother and more optimized experience. 

## tldr 
 
> A simple wrapper that runs Winetricks commands for Proton enabled games.
> More information: <https://github.com/Matoking/protontricks>.

- Run the protontricks GUI:

`protontricks --gui`

- Run Winetricks for a specific game:

`protontricks {{appid}} {{winetricks_args}}`

- Run a command within a game's installation directory:

`protontricks -c {{command}} {{appid}}`

- [l]ist all installed games:

`protontricks -l`

- [s]earch for a game's App ID by name:

`protontricks -s {{game_name}}`

- Show the protontricks help message:

`protontricks --help`
