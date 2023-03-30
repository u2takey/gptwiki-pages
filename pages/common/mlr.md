# mlr 
## chatgpt 
The "mlr" command refers to Miller, a command-line tool used for processing structured text data such as CSV, TSV, and JSON files. 

Using mlr, you can perform various data manipulation tasks such as filtering, sorting, joining, aggregating, and formatting data.

Here are some common mlr commands with a brief explanation:

- mlr cut: To select specific columns from a CSV file, you can use the "cut" command. For example, "mlr cut -f column1,column3 input.csv" will output only columns 1 and 3 from a CSV file called "input.csv".

- mlr filter: This command lets you filter rows based on certain conditions. For example, "mlr filter '$age > 30' input.csv" will filter out all rows where the "age" column is less than or equal to 30.

- mlr join: To combine two CSV files based on a common column, you can use the "join" command. For example, "mlr join -j common_column input1.csv input2.csv" will join two CSV files called "input1" and "input2" based on the "common_column".

- mlr stats: This command lets you calculate various statistics on your data. For example, "mlr stats -a min,max,mean -f value input.csv" will calculate the minimum, maximum, and mean values for the "value" column in a CSV file called "input.csv".

These are just a few examples of what you can do with the mlr command. For more information on the mlr command and its various options, you can refer to the mlr documentation. 

## tldr 
 
> Miller is like `awk`, `sed`, `cut`, `join`, and `sort` for name-indexed data such as CSV, TSV, and tabular JSON.
> More information: <https://johnkerl.org/miller/doc>.

- Pretty-print a CSV file in a tabular format:

`mlr --icsv --opprint cat {{example.csv}}`

- Receive JSON data and pretty print the output:

`echo '{"hello":"world"}' | mlr --ijson --opprint cat`

- Sort alphabetically on a field:

`mlr --icsv --opprint sort -f {{field}} {{example.csv}}`

- Sort in descending numerical order on a field:

`mlr --icsv --opprint sort -nr {{field}} {{example.csv}}`

- Convert CSV to JSON, performing calculations and display those calculations:

`mlr --icsv --ojson put '${{newField1}} = ${{oldFieldA}}/${{oldFieldB}}' {{example.csv}}`

- Receive JSON and format the output as vertical JSON:

`echo '{"hello":"world", "foo":"bar"}' | mlr --ijson --ojson --jvstack cat`

- Filter lines of a compressed CSV file treating numbers as strings:

`mlr --prepipe 'gunzip' --csv filter -S '${{fieldName}} =~ "{{regular_expression}}"' {{example.csv.gz}}`
