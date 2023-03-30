# dvc config 
## chatgpt 
The "dvc config" command is used to view or modify the configuration settings of DVC (Data Version Control). DVC is an open-source tool used for managing machine learning experiments and data science projects. 

When executed, the "dvc config" command provides a list of all the configuration settings that have been set up on the system. These settings are stored in a YAML file called "config" that is located in the ".dvc" directory.

You can modify any of the configuration settings by using the appropriate command-line option. For example, to set the cache directory location path to "/tmp/dvc-cache", you can use the command "dvc config cache.dir /tmp/dvc-cache".

There are several configuration settings that can be modified, such as the remote storage location, cache directory, default target path, and log verbosity level. By modifying these settings, you can customize the behavior of DVC on your system. 

Overall, the "dvc config" command is an essential tool for working with DVC as it allows you to view and modify the configuration settings, which helps to streamline the data management process. 

## tldr 
 
> Low level command to manage custom configuration options for dvc repositories.
> These configurations can be on project, local, global, or system level.
> More information: <https://dvc.org/doc/command-reference/config>.

- Get the name of the default remote:

`dvc config core.remote`

- Set the project's default remote:

`dvc config core.remote {{remote_name}}`

- Unset the project's default remote:

`dvc config --unset core.remote`

- Get the config value for a specified key for the current project:

`dvc config {{key}}`

- Set the config value for a key on a project level:

`dvc config {{key}} {{value}}`

- Unset a project level config value for a given key:

`dvc config --unset {{key}}`

- Set a local, global, or system level config value:

`dvc config --local/global/system {{key}} {{value}}`
