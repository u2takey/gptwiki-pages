# tlmgr conf 
## chatgpt 
The `tlmgr conf` command is used in TeX Live to access and modify configuration settings for the TeX Live Manager, which is the primary tool for managing TeX Live installations.

When you run `tlmgr conf`, it will display a list of configuration variables and their current values. These variables control various aspects of how TeX Live operates, such as the location of the TeX Live installation directory, the location of temporary files, and the behavior of the package update system.

You can use the `tlmgr conf` command to modify these variables by specifying new values for them as command-line options. For example, you might use `tlmgr conf texmfdir /usr/local/texlive/2021/texmf-dist` to change the directory where TeX Live stores its package files.

Overall, the `tlmgr conf` command provides a way to customize the behavior of TeX Live and ensure that it meets your specific needs. 

## tldr 
 
> Manage the TeX Live configuration.
> More information: <https://www.tug.org/texlive/tlmgr.html>.

- Show the current TeX Live configuration:

`tlmgr conf`

- Show the current `texmf`, `tlmgr`, or `updmap` configuration:

`tlmgr conf {{texmf|tlmgr|updmap}}`

- Show only a specific configuration option:

`tlmgr conf {{texmf|tlmgr|updmap}} {{configuration_key}}`

- Set a specific configuration option:

`tlmgr conf {{texmf|tlmgr|updmap}} {{configuration_key}} {{value}}`

- Delete a specific configuration option:

`tlmgr conf {{texmf|tlmgr|updmap}} --delete {{configuration_key}}`

- Disable the execution of system calls via `\write18`:

`tlmgr conf texmf {{shell_escape}} {{0}}`

- Show all additional `texmf` trees:

`tlmgr conf auxtrees show`
