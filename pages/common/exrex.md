# exrex 
## chatgpt 
Exrex is a Python command line tool used to generate all possible matching strings based on a given regular expression pattern. The tool creates permutations of strings based on a set of characters included in the regular expression pattern. Exrex is useful for developing test cases for applications or scripts that require input validation based on regular expressions. 

Here's an example of how to use exrex:
Suppose you want to generate all possible phone numbers in the format 555-XXXX, where X represents any digit. The regular expression pattern for this format would be: "555-\d\d\d\d". You can use exrex to generate a list of all possible phone numbers that match this pattern by typing the following command in your terminal:

exrex '555-\d\d\d\d'

Exrex will output all possible matching strings, such as "555-0000", "555-0001", etc.

Overall, exrex is a powerful tool for generating test cases quickly and easily based on regular expressions. 

## tldr 
 
> Generate all/random matching strings for a regular expression.
> It can also simplify regular expressions.
> More information: <https://github.com/asciimoo/exrex>.

- Generate all possible strings that match a regular expression:

`exrex '{{regular_expression}}'`

- Generate a random string that matches a regular expression:

`exrex --random '{{regular_expression}}'`

- Generate at most 100 strings that match a regular expression:

`exrex --max-number {{100}} '{{regular_expression}}'`

- Generate all possible strings that match a regular expression, joined by a custom delimiter string:

`exrex --delimiter "{{, }}" '{{regular_expression}}'`

- Print count of all possible strings that match a regular expression:

`exrex --count '{{regular_expression}}'`

- Simplify a regular expression:

`exrex --simplify '{{ab|ac}}'`

- Print eyes:

`exrex '{{[oO0](_)[oO0]}}'`

- Print a boat:

`exrex '{{( {20}(\| *\\|-{22}|\|)|\.={50}| ( ){0,5}\\\.| {12}~{39})}}'`
