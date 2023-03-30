# lua 
## chatgpt 
The "lua" command is used to execute Lua scripts on the command line. Lua is an open-source, lightweight, embeddable scripting language that is often used in video game development, web development, and other applications.

The syntax for using the "lua" command is simple:

```
lua [options] [script [args]]
```

The options can be used to set various parameters, such as the amount of memory allocated for Lua or whether to run the script in debug mode.

The "script" parameter specifies the Lua script file to execute.

The "args" parameter can be used to pass command-line arguments to the script.

For example, to execute a script called "myscript.lua" with the command-line argument "hello", you would use the following command:

```
lua myscript.lua hello
```

This would execute the "myscript.lua" file using the Lua interpreter, passing the "hello" argument to the script.

Overall, the "lua" command provides a simple and powerful way to run Lua scripts on the command line, making it a valuable tool for Lua programmers and developers. 

## tldr 
 
> A powerful, light-weight embeddable programming language.
> More information: <https://www.lua.org>.

- Start an interactive Lua shell:

`lua`

- Execute a Lua script:

`lua {{script_name.lua}} {{--optional-argument}}`

- Execute a Lua expression:

`lua -e '{{print( "Hello World" )}}'`
