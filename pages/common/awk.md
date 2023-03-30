# awk 
## chatgpt 
`awk` is a text processing tool that is used to perform a variety of data manipulation tasks in Unix/Linux systems. It can be used to extract specific rows and columns from a file, perform text transformations, and calculate summary statistics, among other things.

The basic syntax for `awk` is as follows:

```
awk 'pattern {action}' file
```

Here, the `pattern` is a regular expression that specifies what lines of text to process, and the `action` is a set of commands to perform on those lines.

For example, to print the first column of a file called `data.txt`, you could use the following `awk` command:

```
awk '{print $1}' data.txt
```

In this case, the pattern is empty, which means that the action will be applied to all lines in the file. The action is simply to print the first column of each line (which is denoted by `$1`).

You can also use `awk` to perform more complex operations on the data. For example, to calculate the average value of the second column in `data.txt`, you could use:

```
awk '{ sum += $2 } END { print sum / NR }' data.txt
```

Here, the `sum` variable is initialized to zero, and then incremented by the value of the second column on each line. After all lines have been processed, the `END` keyword is used to perform a final calculation (in this case, to divide the sum by the number of lines, which is represented by the `NR` built-in variable).

`awk` is a powerful tool that can be used for a wide range of text processing tasks, and it is a valuable addition to any Unix/Linux user's toolkit. 

## tldr 
 
> A versatile programming language for working on files.
> More information: <https://github.com/onetrueawk/awk>.

- Print the fifth column (a.k.a. field) in a space-separated file:

`awk '{print $5}' {{path/to/file}}`

- Print the second column of the lines containing "foo" in a space-separated file:

`awk '/{{foo}}/ {print $2}' {{path/to/file}}`

- Print the last column of each line in a file, using a comma (instead of space) as a field separator:

`awk -F ',' '{print $NF}' {{path/to/file}}`

- Sum the values in the first column of a file and print the total:

`awk '{s+=$1} END {print s}' {{path/to/file}}`

- Print every third line starting from the first line:

`awk 'NR%3==1' {{path/to/file}}`

- Print different values based on conditions:

`awk '{if ($1 == "foo") print "Exact match foo"; else if ($1 ~ "bar") print "Partial match bar"; else print "Baz"}' {{path/to/file}}`

- Print all lines where the 10th column value equals the specified value:

`awk '($10 == value)'`

- Print all the lines which the 10th column value is between a min and a max:

`awk '($10 >= min_value && $10 <= max_value)'`
