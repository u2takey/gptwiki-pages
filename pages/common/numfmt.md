# numfmt 
## chatgpt 
The `numfmt` command is used to convert numbers in one format to another format using the command line interface. It can be used to convert numbers between different units of measurement, such as bytes to gigabytes, or between different number systems, such as decimal to binary.

Here are some of the options available with `numfmt`:

- `-d` or `--delimiter`: Specifies the delimiter to be used when formatting output numbers. The default delimiter is a comma.
- `-f` or `--format`: Specifies a specific output format. For example, to format numbers as percentages, use the option `-f %`.
- `-i` or `--to-incremental`: Formats output numbers in an incremental sequence. For example, 1, 2, 3, etc.
- `-l` or `--locale`: Specifies a specific locale to use for formatting output numbers. By default, the system's locale is used.
- `-p` or `--padding`: Specifies the number of digits a number should have when formatted. For example, to pad a number with leading zeros to make it 10 digits long, use `-p 10`.
- `-u` or `--from-unit`: Specifies the unit of measurement to convert from. For example, to convert bytes to megabytes, use `-u b` for bytes and `-u m` for megabytes.
- `-t` or `--to-unit`: Specifies the unit of measurement to convert to. For example, to convert bytes to megabytes, use `-t m` for megabytes.


Overall, the `numfmt` command provides a quick and easy way to convert numbers in different formats, and supports many different options to provide flexibility in the conversions. 

## tldr 
 
> Convert numbers to and from human-readable strings.
> More information: <https://www.gnu.org/software/coreutils/numfmt>.

- Convert 1.5K (SI Units) to 1500:

`numfmt --from={{si}} {{1.5K}}`

- Convert 5th field (1-indexed) to IEC Units without converting header:

`ls -l | numfmt --header={{1}} --field={{5}} --to={{iec}}`

- Convert to IEC units, pad with 5 characters, left aligned:

`du -s * | numfmt --to={{iec}} --format="{{%-5f}}"`
