# erl 
## chatgpt 
The "erl" command is used to launch the Erlang Shell in a command-line interface. Erlang shell is an interactive environment that allows developers to test and run Erlang programs.

When you enter the "erl" command in the terminal, the Erlang Shell is launched, and you can start interacting with it. The shell prompt will appear as "Erlang" or "Eshell" followed by version information.

Once inside the Erlang shell, you can execute various commands, define functions, create variables, and interact with the Erlang runtime environment. The shell provides features such as auto-completion, history, and context-sensitive help to facilitate the development process.

Some common commands that can be executed in the Erlang shell include:

- c(ModuleName): Compiles a module.
- l(ModuleName): Loads a module and makes its functions available.
- q(): Quits the Erlang shell.

In summary, the erl command launches the Erlang Shell, which is an interactive environment for developing, testing, and running Erlang programs. 

## tldr 
 
> Run and manage programs in the Erlang programming language.
> More information: <https://www.erlang.org>.

- Compile and run sequential Erlang program as a common script and then exit:

`erlc {{files}} && erl -noshell '{{mymodule:myfunction(arguments)}}, init:stop().'`

- Connect to a running Erlang node:

`erl -remsh {{nodename}}@{{hostname}} -sname {{custom_shortname}} -hidden -setcookie {{cookie_of_remote_node}}`

- Tell the Erlang shell to load modules from a directory:

`erl -pa {{directory_with_beam_files}}`
