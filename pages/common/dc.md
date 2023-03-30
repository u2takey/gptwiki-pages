# dc 
## chatgpt 
The "dc" command stands for Desktop Calculator. It is a command-line utility that provides a command-line interface for performing basic arithmetic operations.

Once dc is started, it runs in interactive mode, accepting input from standard input (usually the keyboard) or from a file, and producing output to standard output (usually the console). The basic syntax for dc is as follows:

dc [options] [file]

Here, options refer to any optional parameters that can be used to modify the behavior of dc, while file refers to the name of the file containing the expressions to be evaluated by dc. If no file is specified, dc runs in interactive mode and waits for input from the user.

To use dc, you need to enter an input expression, followed by the "Enter" key. You can use basic arithmetic operators like addition (+), subtraction (-), multiplication (*), and division (/), and other operations that manipulate the stack, including the stack-push operator ("d"), the stack-duplicate operator ("f"), and the stack-exchange operator ("r").

For instance, you can enter the following expression to perform a basic arithmetic operation in dc:

$ dc
2 3 + p

Here, the "2 3 +" expression adds 2 and 3 together, and the "p" command prints the result to the console. The output of this command will be "5". 

## tldr 
 
> An arbitrary precision calculator. Uses reverse polish notation (RPN).
> See also: `bc`.
> More information: <https://www.gnu.org/software/bc/manual/dc-1.05/html_mono/dc.html>.

- Start an interactive session:

`dc`

- Execute a script:

`dc {{path/to/script.dc}}`

- Calculate an expression with the specified scale:

`dc --expression='{{10}} k {{5 3 /}} p'`

- Calculate 4 times 5 (4 5 *), subtract 17 (17 -), and [p]rint the output:

`dc --expression='4 5 * 17 - p'`

- Set number of decimal places to 7 (7 k), calculate 5 divided by -3 (5 _3 /) and [p]rint:

`dc --expression='7 k 5 _3 / p'`

- Calculate the golden ratio, phi: set number of decimal places to 100 (100 k), square root of 5 (5 v) plus 1 (1 +), divided by 2 (2 /), and [p]rint result:

`dc --expression='100 k 5 v 1 + 2 / p'`
