# choose 
## chatgpt 
As an AI language model, I can explain the "Choose" command in general terms, but I would need a context to provide a specific explanation. In programming languages such as SQL, choose is typically used in conditional statements to select a specific course of action based on a given condition. For example, the SQL syntax:

SELECT column_name(s)
FROM table_name
WHERE condition
ORDER BY column_name(s)

uses the "WHERE" clause to choose specific data based on a condition that is evaluated. Similarly, choose can be used in other languages such as Python, where you might use the if/else statement to choose which code block to execute based on a condition.

Overall, the "Choose" command is a way for programmers to provide a programmatic decision-making logic to their code. 

## tldr 
 
> A human-friendly and fast alternative to cut and (sometimes) awk.
> More information: <https://github.com/theryangeary/choose>.

- Print the 5th item from a line (starting from 0):

`choose {{4}}`

- Print the first, 3rd, and 5th item from a line, where items are separated by ':' instead of whitespace:

`choose --field-separator '{{:}}' {{0}} {{2}} {{4}}`

- Print everything from the 2nd to 5th item on the line, including the 5th:

`choose {{1}}:{{4}}`

- Print everything from the 2nd to 5th item on the line, excluding the 5th:

`choose --exclusive {{1}}:{{4}}`

- Print the beginning of the line to the 3rd item:

`choose :{{2}}`

- Print all items from the beginning of the line until the 3rd item (exclusive):

`choose --exclusive :{{2}}`

- Print all items from the 3rd to the end of the line:

`choose {{2}}:`

- Print the last item from a line:

`choose {{-1}}`
