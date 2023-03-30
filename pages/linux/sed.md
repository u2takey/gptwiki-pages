# sed 
## chatgpt 
`sed` is a powerful text editor used in Unix-based operating systems that allows for modifying and manipulating text within files or standard input/output. It is short for "stream editor." 

The basic syntax of `sed` is:

```
sed [options] [script] [input file]
```

Here's what each part of the syntax represents:

- `options`: optional flags that modify the behavior of the `sed` command. These can include suppressing output (-n), performing case-insensitive substitutes (-i), or using extended regular expressions (-E).
- `script`: the commands to execute on the input file. Scripts can include a combination of commands, such as substitution (s), deletion (d), printing (p), or appending (a).
- `input file`: the file(s) on which to perform the edit. If none is specified, input is read from standard input.

Here are some basic examples of how to use `sed`:

- Substitute 'foo' with 'bar' in an input file and print the output to the console:
  
  ```
  sed 's/foo/bar/g' input.txt
  ```
  
- Delete all lines containing 'foo' in an input file and print the output to the console:

  ```
  sed '/foo/d' input.txt
  ```

- Append a line after each occurrence of 'foo' in an input file and print the output to the console:

  ```
  sed '/foo/a This line is appended after "foo"' input.txt
  ```

- Ignore case when substituting 'foo' with 'bar' in an input file and save the changes to the file:

  ```
  sed -i 's/foo/bar/gI' input.txt
  ```

Overall, `sed` provides a flexible and efficient way to modify text data in a variety of different contexts. 

## tldr 
 
> Edit text in a scriptable manner.
> See also: `awk`, `ed`.
> More information: <https://www.gnu.org/software/sed/manual/sed.html>.

- Replace all `apple` (basic regex) occurrences with `mango` (basic regex) in all input lines and print the result to `stdout`:

`{{command}} | sed 's/apple/mango/g'`

- Execute a specific script [f]ile and print the result to `stdout`:

`{{command}} | sed -f {{path/to/script.sed}}`

- Replace all `apple` (extended regex) occurrences with `APPLE` (extended regex) in all input lines and print the result to `stdout`:

`{{command}} | sed -E 's/(apple)/\U\1/g'`

- Print just a first line to `stdout`:

`{{command}} | sed -n '1p'`

- Replace all `apple` (basic regex) occurrences with `mango` (basic regex) in a specific file and overwrite the original file in place:

`sed -i 's/apple/mango/g' {{path/to/file}}`
