# powerprofilesctl 
## chatgpt 
powerprofilesctl is a command that is used to manage power profiles on Linux systems. It allows users to control how their system manages power consumption and performance.

The powerprofilesctl command can be used to switch between different power profiles, which will affect how the system uses resources such as CPU, memory, and disk usage. This can be useful for users who want to optimize their system's performance for certain tasks, such as gaming or video editing.

The command can also be used to list available power profiles and get detailed information on each profile, including its name, description, and options.

Some of the common options that can be used with the powerprofilesctl command include:

-switch: This option is used to switch to a specific power profile. The user must provide the name of the profile they want to switch to.

-list: This option is used to list all available power profiles on the system.

-info: This option is used to get detailed information on a specific power profile, including its name, description, and options.

-help: This option is used to display a help message that explains the available options for the powerprofilesctl command.

Overall, the powerprofilesctl command is a powerful tool that allows users to manage power profiles on Linux systems in order to optimize performance and conserve energy. 

## tldr 
 
> Make power profiles handling available over D-Bus.
> More information: <https://gitlab.freedesktop.org/hadess/power-profiles-daemon/>.

- List available power profiles:

`powerprofilesctl list`

- Set a specific power profile:

`powerprofilesctl set {{profile_name}}`
