# uniq 
## chatgpt 
The Unix command `uniq` is a basic filtering command which is used to remove the repeated lines from a text file or standard input. It is a useful command when you have a file with duplicates lines and you want to remove them to make it more readable or processable. It can also be used to count and manipulate the occurrences of duplicate lines.

Syntax:

The syntax for `uniq` is as follows:

```
uniq [OPTION]... [INPUT [OUTPUT]]
```

Options:

The following are the most commonly used options for `uniq` command:

- `-c` : displays the number of repeated lines along with the actual line.
- `-d` : displays only the duplicate lines.
- `-i` : ignores case distinctions between lines.
- `-u` : displays only the unique lines (i.e., removes duplicate lines).
- `-f N` : skips first N fields before checking for duplicates.
- `-s N` : skips first N characters before checking for duplicates.

Examples:

1. To remove duplicate lines from a file `file1.txt`, use:

```
$ uniq file1.txt
```

2. To count the number of occurrences of each duplicate line in a file `file2.txt`, use:

```
$ uniq -c file2.txt
```

3. To remove duplicate lines from a file `file3.txt` and save the output to a new file `output.txt`, use:

```
$ uniq file3.txt > output.txt
```

4. To ignore case distinctions and remove duplicate lines from a file `file4.txt`, use:

```
$ uniq -i file4.txt
```

5. To skip the first 3 fields and remove duplicate lines from a file `file5.txt`, use:

```
$ uniq -f 3 file5.txt
```

6. To skip the first 10 characters and remove duplicate lines from a file `file6.txt`, use:

```
$ uniq -s 10 file6.txt
``` 

## tldr 
 
> Output the unique lines from the given input or file.
> Since it does not detect repeated lines unless they are adjacent, we need to sort them first.
> More information: <https://www.gnu.org/software/coreutils/uniq>.

- Display each line once:

`sort {{path/to/file}} | uniq`

- Display only unique lines:

`sort {{path/to/file}} | uniq -u`

- Display only duplicate lines:

`sort {{path/to/file}} | uniq -d`

- Display number of occurrences of each line along with that line:

`sort {{path/to/file}} | uniq -c`

- Display number of occurrences of each line, sorted by the most frequent:

`sort {{path/to/file}} | uniq -c | sort -nr`
