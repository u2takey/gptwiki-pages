# tmuxinator 
## chatgpt 
tmuxinator is a command-line tool used to easily create and manage complex tmux sessions. Tmux is a terminal multiplexer that allows users to create multiple sessions, each with multiple windows and panes.

With tmuxinator, users can create a YAML file containing detailed session and window configurations, including commands to run upon creation. These configuration files can be easily shared and reused among team members, making it easier to collaborate on complex projects.

Once a configuration file is created, users can start the tmux session with a single command using the tmuxinator command followed by the name of the configuration file. The tmuxinator tool takes care of all the necessary tmux commands to create and configure the session according to the configuration file.

In summary, the tmuxinator command is a powerful tool for managing tmux sessions, allowing for easy creation and management of complex configurations. 

## tldr 
 
> Create and manage tmux sessions easily.
> More information: <https://github.com/tmuxinator/tmuxinator>.

- Create a new project:

`tmuxinator new {{project}}`

- Edit a project:

`tmuxinator edit {{project}}`

- List projects:

`tmuxinator list`

- Start a tmux session based on project:

`tmuxinator start {{project}}`

- Stop a project's tmux session:

`tmuxinator stop {{project}}`
