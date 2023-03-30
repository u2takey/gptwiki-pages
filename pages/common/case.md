# case 
## chatgpt 
The command "case" is a conditional statement in many programming languages that allows for multiple possible paths of code execution depending on the value of a variable or expression. 

In its basic form, the "case" statement is constructed with the following syntax:

```
case expression
when value1
  statement1
when value2
  statement2
...
when valueN
  statementN
[else
  statementX]
end
```

The "expression" specifies the variable or expression that is being evaluated, and the subsequent "when" statements compare the expression to different possible values. 

If the expression matches a particular value, then the corresponding "statement" is executed. If no "when" statement matches the expression, then the "else" block (if provided) is executed instead. 

For example, suppose we have a program that accepts a user's age and then outputs a message based on that age. We could use a "case" statement like this:

```
age = 25

case age
when 0..17
  puts "You are a minor."
when 18..64
  puts "You are an adult."
when 65..120
  puts "You are a senior citizen."
else
  puts "Invalid age input."
end
```

In this example, the "age" variable is evaluated by the "case" statement, and the corresponding "puts" statement is executed based on the value of "age". If "age" is less than or equal to 17, the first message is displayed. If "age" is between 18 and 64 (inclusive), the second message is displayed. If "age" is between 65 and 120 (inclusive), the third message is displayed. If "age" does not match any of these ranges, then the "else" block is executed and an error message is displayed. 

## tldr 
 
> Branch based on the value of an expression.
> More information: <https://manned.org/case>.

- Match a variable against string literals to decide which command to run:

`case {{$tocount}} in {{words}}) {{wc -w README}}; ;; {{lines}}) {{wc -l README}}; ;; esac`

- Combine patterns with |, use * as a fallback pattern:

`case {{$tocount}} in {{[wW]|words}}) {{wc -w README}}; ;; {{[lL]|lines}}) {{wc -l README}}; ;; *) {{echo "what?"}}; ;; esac`
