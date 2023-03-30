# loc 
## chatgpt 
As an AI language model, I can provide the general definition of the `loc` command, which is a method used to retrieve rows and columns from a Pandas DataFrame or Series object in Python. 

The `loc` command stands for "location" and is used to select rows or columns from a DataFrame or labeled Series using labels or boolean arrays. It is especially useful when dealing with large datasets and when selecting rows or columns based on specific criteria.

The basic syntax for using the `loc` command in Python is:

```
df.loc[row_indexer, column_indexer]
```

Here, `row_indexer` and `column_indexer` are the labels of the rows and columns to be retrieved from the DataFrame or Series object. 

For instance, to select all rows with the label "A" and columns "X" and "Y" from a DataFrame called `df`, you can use the following code:

```
df.loc['A', ['X', 'Y']]
```

The `loc` command can also take boolean arrays to select rows or columns based on specific criteria. For instance, to select all rows where the value in the "X" column is greater than 5 and less than 10, you can use the following code:

```
df.loc[(df['X'] > 5) & (df['X'] < 10)]
```

In summary, the `loc` command in Python is a powerful method used to retrieve rows and columns from a DataFrame or Series object using labels or boolean arrays. It is a key tool in data analysis and manipulation. 

## tldr 
 
> Tool written in Rust that counts lines of code.
> More information: <https://github.com/cgag/loc>.

- Print lines of code in the current directory:

`loc`

- Print lines of code in the target directory:

`loc {{path/to/directory}}`

- Print lines of code with stats for individual files:

`loc --files`

- Print lines of code without .gitignore (etc.) files (e.g. two -u flags will additionally count hidden files and dirs):

`loc -u`
