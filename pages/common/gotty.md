# gotty 
## chatgpt 
Goty is a terminal emulator and a utility tool that allows users to access their terminal sessions over the web. The command "gotty" is used to run the Goty server and open a terminal session in a web browser. 

The syntax for the command is as follows:

gotty [options] [command [arg ...]]

The "options" section includes various configuration options that can be used to customize the behavior of the Goty server, while the "command [arg ...]" section specifies the command that should be executed in the terminal session.

Some of the commonly used options for the Goty command include the following:

- -p, --port: Specifies the host port on which the Goty server should listen.
- -w, --permit-write: Allows users to write to the terminal session.
- -c, --credential: Sets a username and password for authenticating users.
- -h, --help: Displays a list of available command-line options and their descriptions.

Overall, the gotty command is a powerful tool that allows users to access their terminal sessions from anywhere and on any device with a web browser. 

## tldr 
 
> Share your terminal as a web application.
> More information: <https://github.com/yudai/gotty>.

- Share result of command:

`gotty {{command}}`

- Share with write permission:

`gotty -w {{shell}}`

- Share with credential (Basic Auth):

`gotty -w -c {{username}}:{{password}} {{shell}}`
