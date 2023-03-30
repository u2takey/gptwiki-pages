# guile 
## chatgpt 
Guile is a programming language interpreter that is primarily designed to help developers in creating and running Scheme programs or Guile extensions that use Scheme as the base language.

When you enter the command `guile` in a terminal or command prompt, it launches the Guile interpreter prompt, where you can type scheme language commands and have them executed immediately.

Once the interpreter prompt is launched, you can start typing in Scheme code, and the interpreter will execute it on the fly as you type it in. It's important to note that Scheme is a Lisp-based language, and so the syntax is different from that of other programming languages.

Here are some examples of what you can do with Guile:

1. Calculate simple math expressions:

```
guile> (+ 2 2)
4
guile> (* 5 8)
40
```

2. Define and manipulate variables:

```
guile> (define name "John")
guile> name
"John"
guile> (string-append "My name is " name)
"My name is John"
```

3. Write and call simple functions:

```
guile> (define (add-two x) (+ x 2))
guile> (add-two 5)
7
```

4. Use built-in Guile procedures to manipulate lists, strings, and more:

```
guile> (string-split "hello world" " ")
("hello" "world")
guile> (list-ref '(1 2 3) 2)
3
```

In summary, the `guile` command launches an interpreter for the Guile programming language, which allows developers to execute Scheme code in real-time. With Guile, developers can write functions, manipulate data types, and use built-in procedures to interact with different types of data such as strings or lists. 

## tldr 
 
> Guile Scheme interpreter.
> More information: <https://www.gnu.org/software/guile>.

- Start a REPL (interactive shell):

`guile`

- Execute the script in a given Scheme file:

`guile {{script.scm}}`

- Execute a Scheme expression:

`guile -c "{{expression}}"`

- Listen on a port or a Unix domain socket (the default is port 37146) for remote REPL connections:

`guile --listen={{port_or_socket}}`
