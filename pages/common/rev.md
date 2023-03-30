# rev 
## chatgpt 
The `rev` command is a Linux/Unix command that is used to reverse the order of characters in each line of a file. It simply prints the output of a file in reverse order.

Syntax: `rev [option] [file]`

Options:
- `-V` — prints the version of `rev`.
- `-h` — prints the help message.
- `-c` — prints the characters of the file in reverse order.
- `-t` — preserves the tabs in the output.
- `--help` — displays the help message and exits.
- `--version` — shows the version of `rev`.

Example usage:

1. To reverse the order of characters in each line of a file:
   
   Command: `rev file.txt`
   
   Output: 
   ```
   elloC naM ot emocleW
   redloH dna kooL
   .yltnecer tnemtrapeD eriH
   ```
   
2. To reverse a string:
   
   Command: `echo "Hello World" | rev`
   
   Output: `dlroW olleH`

3. To reverse the order of characters in each line of multiple files:
   
   Command: `rev file1.txt file2.txt`
   
   Output for `file1.txt`:
   ```
   elloC naM ot emocleW
   redloH dna kooL
   .yltnecer tnemtrapeD eriH
   ```
   
   Output for `file2.txt`:
   ```
   gniK kooL si siht
   naM yM si eman
   .tsac taht ffO
   ``` 

## tldr 
 
> Reverse a line of text.
> More information: <https://manned.org/rev>.

- Reverse the text string "hello":

`echo "hello" | rev`

- Reverse an entire file and print to `stdout`:

`rev {{path/to/file}}`
