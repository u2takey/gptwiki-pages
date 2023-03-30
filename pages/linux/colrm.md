# colrm 
## chatgpt 
The "colrm" command is a Unix/Linux command used to remove columns from a text file. 

The syntax of the "colrm" command is as follows:

colrm [start] [stop]

Here, "start" is the column number from where you want to start removing, and "stop" is the column number at which you want to stop removing from the text file.

For example, if you have a file called "sample.txt" with the following content:

```
This is a sample text file.
It contains multiple lines of text.
```

If you want to remove the first four columns from the file, you would use the following command:

```
colrm 1 4 sample.txt
```

The output of this command would be:

```
is a sample text file.
 contains multiple lines of text.
```

The "colrm" command can be useful in situations where you have a large text file with unwanted columns or if you need to extract specific columns from a text file. 

## tldr 
 
> Remove columns from `stdin`.
> More information: <https://manned.org/colrm>.

- Remove first column of `stdin`:

`colrm {{1 1}}`

- Remove from 3rd column till the end of each line:

`colrm {{3}}`

- Remove from the 3rd column till the 5th column of each line:

`colrm {{3 5}}`
