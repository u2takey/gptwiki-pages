# sbcl 
## chatgpt 
sbcl is a command used to start the Steel Bank Common Lisp (SBCL) interpreter or compiler. SBCL is a high-performance implementation of Common Lisp that is designed to be fast and efficient while also offering a comprehensive set of features for developing Lisp-based applications.

When you execute the sbcl command, the SBCL shell will launch, providing a prompt where you can enter Lisp expressions and commands. You can use the sbcl command to interactively develop and test Lisp code, or you can use it to compile Lisp source code into standalone executables or libraries.

Some common options that can be used with the sbcl command include:

- --core <file>: Specifies the path to a precompiled SBCL image to use instead of the default image.
- --load <file>: Loads a Lisp source file into the SBCL environment.
- --eval <expr>: Evaluates a Lisp expression within the SBCL environment.
- --quit: Exits the SBCL environment.

Overall, the sbcl command is an essential tool for Lisp programmers and developers who need a fast and reliable implementation of the Common Lisp language. 

## tldr 
 
> High performance Common Lisp compiler.
> More information: <http://www.sbcl.org/>.

- Start a REPL (interactive shell):

`sbcl`

- Execute a Lisp script:

`sbcl --script {{path/to/script.lisp}}`
