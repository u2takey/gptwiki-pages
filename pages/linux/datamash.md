# datamash 
## chatgpt 
Datamash is a command-line tool for statistical analysis and manipulation of text/csv files. 

Here are some common use cases and explanations of datamash commands:

1. Basic mathematical operations: 
- `datamash sum 1` will add up values in the first column
- `datamash mean 3` will calculate the mean of values in the third column
- `datamash min 2` will find the minimum value in the second column

2. Grouping/aggregation:
- `datamash sum 3 groupby 1` will sum up values in the third column for each unique value in the first column
- `datamash collapse 1,2 count 1 groupby 2` will concatenate values in columns 1 and 2 for each unique value in the second column, and count the number of occurrences of each unique combination
- `datamash transpose` will transpose a set of rows and columns, and calculate various summary statistics for each row/column

3. Data transformation:
- `datamash reverse` will reverse the order of columns in a file
- `datamash paste file1 file2` will paste two files side by side (e.g. horizontally concatenate) based on row number
- `datamash cut -f 1,3,4,6` will cut out columns 1, 3, 4, and 6 from a file

Overall, datamash is a powerful tool for performing a variety of data manipulation and analysis tasks from the command line. 

## tldr 
 
> Tool to perform basic numeric, textual and statistical operations on input textual data files.
> More information: <http://www.gnu.org/software/datamash/>.

- Get max, min, mean and median of a single column of numbers:

`seq 3 | datamash max 1 min 1 mean 1 median 1`

- Get the mean of a single column of float numbers (floats must use "," and not "."):

`echo -e '1.0\n2.5\n3.1\n4.3\n5.6\n5.7' | tr '.' ',' | datamash mean 1`

- Get the mean of a single column of numbers with a given decimal precision:

`echo -e '1\n2\n3\n4\n5\n5' | datamash -R {{number_of_decimals_wanted}} mean 1`

- Get the mean of a single column of numbers ignoring "Na" and "NaN" (literal) strings:

`echo -e '1\n2\nNa\n3\nNaN' | datamash --narm mean 1`
