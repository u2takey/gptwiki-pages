# racket 
## chatgpt 
Racket is an interactive programming language that belongs to the Lisp family. When you enter the command "racket" in your terminal or command prompt, it launches the Racket REPL (Read-Eval-Print Loop) environment, which allows you to enter and execute Lisp code interactively.

The REPL environment enables you to test and experiment with individual expressions or functions, which can help you to develop programs more efficiently. In addition, Racket comes with a rich set of libraries and tools that assist developers in creating complex applications.

Once you're in the Racket REPL environment, you can define variables, functions, or modules, as well as load and evaluate code from files or URLs. The environment also provides various commands and functions that allow you to inspect and manipulate data structures, debug programs, and perform various other tasks.

Overall, the "racket" command is the entry point for launching the Racket programming environment, where you can write, test, and execute Lisp code interactively. 

## tldr 
 
> Racket language interpreter.
> More information: <https://racket-lang.org>.

- Start a REPL (interactive shell):

`racket`

- Execute a Racket script:

`racket {{path/to/script.rkt}}`

- Execute a Racket expression:

`racket --eval "{{expression}}"`

- Run module as a script (terminates option list):

`racket --lib {{module_name}} --main {{arguments}}`

- Start a REPL (interactive shell) for the `typed/racket` hashlang:

`racket -I typed/racket`
