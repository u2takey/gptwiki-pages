# fselect 
## chatgpt 
fselect is a command-line tool used to search and filter files on a Unix or Linux system. It is used to perform searches and filters on files and directories based on specific criteria such as file size, timestamps, owner, permissions, and other attributes.

Syntax:
fselect [options] search_query [directory_path]

Options:
-h: Shows help for fselect
-v: Shows the version number
-l: Lists search and filter options

Search Query:
The search query is a set of rules and clauses used to define the criteria for searching and filtering the files. The query can include logical operators such as AND/OR, wildcards, and regular expressions.

Examples:
1. To search for all files in the home directory owned by the user "john":
fselect -f "user(john)" ~

2. To search for all files modified within the last 24 hours in the /var/log directory:
fselect -f "mtime(-1d..)" /var/log

3. To search for all files with the .txt extension in the /home directory:
fselect -f "name('*.txt')" /home

4. To search for all files over 1MB in size in the /tmp directory:
fselect -f "size(1M..)" /tmp

Overall, fselect is a powerful command-line tool that provides flexible and comprehensive file searching and filtering capabilities. 

## tldr 
 
> Find files with SQL-like queries.
> More information: <https://github.com/jhspetersson/fselect>.

- Select full path and size from temporary or config files in a given directory:

`fselect size, path from {{path/to/directory}} where name = {{'*.cfg'}} or name = {{'*.tmp'}}`

- Find square images:

`fselect path from {{path/to/directory}} where width = height`

- Find old-school rap 320kbps MP3 files:

`fselect path from {{path/to/directory}} where genre = {{Rap}} and bitrate = {{320}} and mp3_year lt {{2000}}`

- Select only the first 5 results and output as JSON:

`fselect size, path from {{path/to/directory}} limit {{5}} into json`

- Use SQL aggregate functions to calculate minimum, maximum and average size of files in a directory:

`fselect "{{MIN(size), MAX(size), AVG(size), SUM(size), COUNT(*)}} from {{path/to/directory}}"`
