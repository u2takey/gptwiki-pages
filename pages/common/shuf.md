# shuf 
## chatgpt 
The `shuf` command in Linux is used to randomly shuffle the lines or entries of a file or standard input. The command is very versatile and can be used to either randomize the lines of a file or the content of a directory.

The basic syntax of the `shuf` command is:

```
shuf [options] [file]
```

Here are some of the common options available with the `shuf` command:

- `-n <num>`: Specifies the number of random lines to be selected from the file or input.
- `-r`: Specifies that the lines should be randomly selected with replacement.
- `-e <items>`: Specifies a list of items to be shuffled. The items should be separated by whitespace.
- `-i <start-end>`: Specifies a range of numbers to be shuffled. The range should be specified as `<start>-<end>`.
- `-z`: Specifies that the input items are separated by a null character instead of a newline.

Examples:

1. Shuffle lines of a file:

```
$ shuf file.txt
```

This command will shuffle the lines of `file.txt` and print them to the standard output.

2. Select a specific number of random lines:

```
$ shuf -n 5 file.txt
```

This command will shuffle the lines of `file.txt` and select 5 of them randomly.

3. Shuffle a list of items:

```
$ shuf -e apple orange banana
```

This command will shuffle the items "apple", "orange", and "banana" and print them to the standard output.

4. Shuffle a range of numbers:

```
$ shuf -i 1-10
```

This command will shuffle the numbers from 1 to 10 and print them to the standard output.

Overall, `shuf` is a very useful command for randomizing data in Linux. 

## tldr 
 
> Generate random permutations.
> More information: <https://www.gnu.org/software/coreutils/shuf>.

- Randomize the order of lines in a file and output the result:

`shuf {{path/to/file}}`

- Only output the first 5 entries of the result:

`shuf --head-count={{5}} {{path/to/file}}`

- Write the output to another file:

`shuf {{path/to/input}} --output={{path/to/output}}`

- Generate 3 random numbers in the range 1-10 (inclusive):

`shuf --head-count={{3}} --input-range={{1-10}} --repeat`
