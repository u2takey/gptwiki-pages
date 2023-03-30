# csvgrep 
## chatgpt 
csvgrep is a command-line tool used to filter and search CSV (Comma Separated Values) files. It allows users to search for specific data within a CSV file using various filtering options. This tool is helpful in streamlining the process of working with large CSV files by efficiently filtering relevant data or extracting specific information.

The syntax for using csvgrep is as follows:

csvgrep [options] [match pattern] [file]

Here, the 'options' parameter refers to various flags that can be used with the command, such as specifying a delimiter, a header, etc. The 'match pattern' parameter refers to the pattern to be matched in the file. The 'file' parameter refers to the CSV file that needs to be filtered.

For example, if you have a CSV file of customer data with fields such as name, address, and phone number, and you want to filter only the records containing a particular name, you can use the following command:

csvgrep -c name -m "John Smith" customers.csv

Here, the '-c' flag is used to specify the column to search for in the CSV file (in this case, the 'name' column), and the '-m' flag is used to specify the match pattern (in this case, "John Smith"). The resulting output will contain only the records that match the specified criteria.

Overall, csvgrep provides a simple way to process and organize large CSV files by filtering specific data and extracting important information. 

## tldr 
 
> Filter CSV rows with string and pattern matching.
> Included in csvkit.
> More information: <https://csvkit.readthedocs.io/en/latest/scripts/csvgrep.html>.

- Find rows that have a certain string in column 1:

`csvgrep -c {{1}} -m {{string_to_match}} {{data.csv}}`

- Find rows in which columns 3 or 4 match a certain regular expression:

`csvgrep -c {{3,4}} -r {{regular_expression}} {{data.csv}}`

- Find rows in which the "name" column does NOT include the string "John Doe":

`csvgrep -i -c {{name}} -m "{{John Doe}}" {{data.csv}}`
