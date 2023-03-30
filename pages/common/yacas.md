# yacas 
## chatgpt 
The command "yacas" refers to a computer software program called Yacas (Yet Another Computer Algebra System). Yacas is an open-source computer algebra system that allows users to perform symbolic manipulation of mathematical equations and expressions. 

When the "yacas" command is executed on the command line or terminal, the Yacas program launches, providing a prompt where users can input mathematical expressions and equations. Yacas supports a wide range of mathematical operations, including algebraic simplification, differentiation, integration, equation solving, and matrix operations.

To use Yacas, users input mathematical expressions into the command prompt, and Yacas will output the result of those expressions. For example, typing "sin(x)^2 + cos(x)^2" into the Yacas prompt would output "1", which is the identity for the pythagorean theorem for sine and cosine.

Overall, the "yacas" command is used to launch the Yacas computer algebra system, which provides a powerful tool for symbolic manipulation of mathematical expressions and equations. 

## tldr 
 
> Yet Another Computer Algebra System.
> More information: <http://www.yacas.org>.

- Start an interactive `yacas` session:

`yacas`

- While in a `yacas` session, execute a statement:

`{{Integrate(x)Cos(x)}};`

- While in a `yacas` session, display an example:

`{{Example()}};`

- Quit from a `yacas` session:

`{{quit}}`

- Execute one or more `yacas` scripts (without terminal or prompts), then exit:

`yacas -p -c {{path/to/script1}} {{path/to/script2}}`

- Execute and print the result of one statement, then exit:

`echo "{{Echo( Deriv(x)Cos(1/x) );}}" | yacas -p -c /dev/stdin`
