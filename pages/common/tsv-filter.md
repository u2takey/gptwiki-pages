# tsv-filter 
## chatgpt 
Unfortunately, as an AI language model, I do not have the context of the tool or program you are referring to with the command "tsv-filter." The command could refer to an option in a specific tool or program, which may have different functionalities and syntax. 

However, generally speaking, a command with the name tsv-filter may be used to filter data in a tab-separated value (TSV) file format. TSV files are a type of text file where data values are separated by a tab character. The tsv-filter command may be used to extract a specific set of rows or columns from a TSV file that meet certain criteria. 

The syntax and options for the tsv-filter command would depend on the specific tool or program it is associated with. It is best to refer to the documentation or help section of the tool to understand the syntax and usage of the tsv-filter command. 

## tldr 
 
> Filter lines of a TSV file by running tests against individual fields.
> More information: <https://github.com/eBay/tsv-utils#tsv-filter>.

- Print the lines where a specific column is numerically equal to a given number:

`tsv-filter -H --eq {{field_name}}:{{number}} {{path/to/tsv_file}}`

- Print the lines where a specific column is [eq]ual/[n]on [e]qual/[l]ess [t]han/[l]ess than or [e]qual/[g]reater [t]han/[g]reater than or [e]qual to a given number:

`tsv-filter --{{eq|ne|lt|le|gt|ge}} {{column_number}}:{{number}} {{path/to/tsv_file}}`

- Print the lines where a specific column is [eq]ual/[n]ot [e]qual/part of/not part of a given string:

`tsv-filter --str-{{eq|ne|in-fld|not-in-fld}} {{column_number}}:{{string}} {{path/to/tsv_file}}`

- Filter for non-empty fields:

`tsv-filter --not-empty {{column_number}} {{path/to/tsv_file}}`

- Print the lines where a specific column is empty:

`tsv-filter --invert --not-empty {{column_number}} {{path/to/tsv_file}}`

- Print the lines that satisfy two conditions:

`tsv-filter --eq {{column_number1}}:{{number}} --str-eq {{column_number2}}:{{string}} {{path/to/tsv_file}}`

- Print the lines that match at least one condition:

`tsv-filter --or --eq {{column_number1}}:{{number}} --str-eq {{column_number2}}:{{string}} {{path/to/tsv_file}}`

- Count matching lines, interpreting first line as a [H]eader:

`tsv-filter --count -H --eq {{field_name}}:{{number}} {{path/to/tsv_file}}`
