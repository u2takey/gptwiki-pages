# update-rc.d 
## chatgpt 
The `update-rc.d` command in Linux is used to manage the startup scripts that run when your system boots. 

When you install a new service or program that needs to start at boot time, it's necessary to create a script that will run when the system starts up. This script is typically written in Bash or another scripting language, and it specifies what the service or program does and how it should be started.

The `update-rc.d` command is used to modify these startup scripts, enabling or disabling them as needed. The command takes various options to change the behavior of the scripts, such as whether they start automatically or need to be started manually.

Here are some of the most common options used with the `update-rc.d` command:

- `update-rc.d -f <script-name> remove`: This option removes the given startup script from the system. This is useful if you no longer need a service or program to start automatically.
- `update-rc.d <script-name> defaults`: This option adds the given startup script to the system's default runlevels, so it will start automatically during a normal system boot.
- `update-rc.d <script-name> disable`: This option disables the given startup script, preventing it from starting automatically during a system boot.
- `update-rc.d -n <script-name> <start-level> <stop-level>`: This option configures the given startup script to start at the specified runlevel and stop at the specified runlevel. This is useful if you need finer control over when a service or program starts and stops.

Overall, the `update-rc.d` command is an important tool for managing the startup scripts that control your system's behavior during boot time. By using this command, you can easily enable or disable services and programs as needed, giving you more control over your Linux system. 

## tldr 
 
> Install and remove services which are System-V style init script links.
> Init scripts are in the `/etc/init.d/`.
> More information: <https://manned.org/update-rc.d>.

- Install a service:

`update-rc.d {{mysql}} defaults`

- Enable a service:

`update-rc.d {{mysql}} enable`

- Disable a service:

`update-rc.d {{mysql}} disable`

- Forcibly remove a service:

`update-rc.d -f {{mysql}} remove`
