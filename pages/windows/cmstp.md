# cmstp 
## chatgpt 
cmstp is a command-line tool used for installing or removing a Connection Manager service profile on a Windows operating system. Connection Manager is a utility that allows users to create and manage virtual private network (VPN) connections, dial-up connections, or other remote access connections to a network.

Syntax:
cmstp /s <full path of the INF file> [/au] [/ns] [/ni] [/nd] [/nv] [/f] [/sms] [/l <full path of the log file>]

Parameters Explanation:

/s: Specifies the full path of the INF file, which contains the Connection Manager service profile information. This parameter is mandatory.

/au: Automatically updates the Connection Manager service profile if the user has administrative rights. This parameter is optional.

/ns: Skips the Connection Manager service profile signature validation. This parameter is optional.

/ni: Prevents the Connection Manager service profile from being installed. This parameter is optional.

/nd: Prevents the Connection Manager service profile from being deleted. This parameter is optional.

/nv: Prevents Connection Manager from displaying the user interface during profile installation. This parameter is optional.

/f: Forces cmstp to overwrite the existing Connection Manager service profile rather than prompting the user for confirmation. This parameter is optional.

/sms: Specifies that the Connection Manager service profile is installed via an SMS script. This parameter is optional.

/l: Specifies the full path of the log file where the installation or removal status will be saved. This parameter is optional.

Examples:

1. To install a Connection Manager service profile –

    cmstp /s "C:\MyServiceProfile.inf"

2. To install a Connection Manager service profile and force overwrite the existing profile –

    cmstp /s "C:\MyServiceProfile.inf" /f

3. To remove a Connection Manager service profile –

    cmstp /s "C:\MyServiceProfile.inf" /ns /nd

In summary, cmstp is a simple and powerful command-line tool used to manage Connection Manager service profiles on Windows. It allows users to install, update, or remove connection profiles from the command prompt. 

## tldr 
 
> A command-line tool for managing connection service profiles.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/cmstp>.

- Install a specific profile:

`cmstp "{{path\to\profile_file}}"`

- Install without creating a desktop shortcut:

`cmstp /ns "{{path\to\profile_file}}"`

- Install without checking for dependencies:

`cmstp /nf "{{path\to\profile_file}}"`

- Only install for the current user:

`cmstp /su "{{path\to\profile_file}}"`

- Install for all users (requires administrator privileges):

`cmstp /au "{{path\to\profile_file}}"`

- Install silently without any prompts:

`cmstp /s "{{path\to\profile_file}}"`

- Uninstall a specific profile:

`cmstp /u "{{path\to\profile_file}}"`

- Uninstall silently without a confirmation prompt:

`cmstp /u /s "{{path\to\profile_file}}"`
