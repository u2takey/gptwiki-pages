# ghci 
## chatgpt 
The "ghci" command is a short form for "Glasgow Haskell Compiler Interactive" and is used to run the Haskell interpreter in the command line interface. When you type "ghci" in your terminal or command-line interface, the Haskell interpreter is launched and you can begin executing Haskell code in real-time.

The GHCi interpreter allows you to interactively test and debug Haskell code, explore the syntax and semantics of the language, load and run Haskell modules, and explore Haskell libraries. In simple terms, ghci is a Read-Eval-Print Loop (REPL) that allows you to enter Haskell expressions and see their results immediately.

Once you type "ghci" in a terminal, you will see a "ghci>" prompt. At this point, you can start writing Haskell code and see the output immediately as you go along. You can define functions, create values, and write expressions that can be evaluated in the interpreter. You can also load external Haskell files and modules using the ":load" command, examine the types of Haskell expressions using the ":type" command, and explore the Haskell environment using various other commands such as ":help", ":quit", and ":info".

Overall, the ghci command is a powerful tool for learning, experimenting, and debugging Haskell code, and is an essential part of any Haskell developer’s toolkit. 

## tldr 
 
> The Glasgow Haskell Compiler's interactive environment.
> More information: <https://downloads.haskell.org/ghc/latest/docs/html/users_guide/ghci.html>.

- Start a REPL (interactive shell):

`ghci`

- Start a REPL and load the specified Haskell source file:

`ghci {{source_file.hs}}`

- Start a REPL and enable a language option:

`ghci -X{{language_option}}`

- Start a REPL and enable some level of compiler warnings (e.g. `all` or `compact`):

`ghci -W{{warning_level}}`

- Start a REPL with a colon-separated list of directories for finding source files:

`ghci -i{{path/to/directory1}}:{{path/to/directory2}}`
