# sed 
## chatgpt 
`sed` is a command-line utility for performing text transformations on a file. The name "sed" stands for "stream editor."

The basic syntax for using `sed` is:

```
sed [options] [commands] [input file]
```

`options` are used to modify the behavior of the command, and are typically preceded by a `-` character.

`commands` are used to specify the text transformations to perform. These are expressed as a series of "sed commands," each of which consists of an address and an action. The address specifies which lines of the input file the command should apply to, while the action specifies how the text should be transformed.

`input file` is the name of the file that will be transformed.

Some common examples of `sed` commands include:

- `s/old/new/`: This command substitutes the first occurrence of `old` with `new` on every line that matches the address.
- `1d`: This command deletes the first line of the input file.
- `/pattern/d`: This command deletes every line that matches the specified pattern.

There are many other `sed` commands and options available, and the tool is extremely powerful and flexible. However, it can also be quite complex to use effectively, especially for complex transformations. 

## tldr 
 
> Edit text in a scriptable manner.
> See also: `awk`, `ed`.
> More information: <https://www.gnu.org/software/sed/manual/sed.html>.

- Replace all `apple` (basic regex) occurrences with `mango` (basic regex) in all input lines and print the result to `stdout`:

`{{command}} | sed 's/apple/mango/g'`

- Execute a specific script [f]ile and print the result to `stdout`:

`{{command}} | sed -f {{path/to/script.sed}}`

- Print just a first line to `stdout`:

`{{command}} | sed -n '1p'`
