# bc 
## chatgpt 
bc stands for "basic calculator" and is a command-line calculator for performing arithmetic operations. It can perform calculations involving basic arithmetic operations, trigonometric functions, logarithms, and more. It can also handle calculations involving large numbers and has support for floating-point arithmetic.

When you run the command "bc" in a terminal, it launches the calculator, and you can start entering expressions to be evaluated (e.g., "2+2"). By default, the calculator assumes that numbers are in base 10, but it can support other bases, such as hexadecimal or octal, by specifying the base before the number (e.g., "0x10" for hexadecimal 16 or "08" for octal 8).

One of the strengths of bc is that it can read input from files or pipes, allowing it to be used in shell scripts or chained together with other commands. For example, you might use "echo '2+2' | bc" to perform a quick calculation in a script or "ls -l | awk '{print $5/1024/1024}' | bc" to convert the size of a file in bytes to megabytes.

Overall, bc is a powerful yet simple tool for performing mathematical calculations from the command line. 

## tldr 
 
> An arbitrary precision calculator language.
> See also: `dc`.
> More information: <https://manned.org/man/bc.1>.

- Start an interactive session:

`bc`

- Start an interactive session with the standard math library enabled:

`bc --mathlib`

- Calculate an expression:

`echo '{{5 / 3}}' | bc`

- Execute a script:

`bc {{path/to/script.bc}}`

- Calculate an expression with the specified scale:

`echo 'scale = {{10}}; {{5 / 3}}' | bc`

- Calculate a sine/cosine/arctangent/natural logarithm/exponential function using `mathlib`:

`echo '{{s|c|a|l|e}}({{1}})' | bc --mathlib`
