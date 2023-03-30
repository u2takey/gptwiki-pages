# gnatprep 
## chatgpt 
The `gnatprep` command is a tool provided by the GNAT Programming Studio (GPS) that is used to generate Ada source code files from template files. It performs text substitution on a given file to produce a new file as output. 

The basic syntax of the `gnatprep` command is as follows:

```
gnatprep [OPTIONS] source_file template_file destination_file
```

Here, `source_file` is the file whose contents need to be replaced, `template_file` is the template file that contains the replacement text, and `destination_file` is the output file where the modified contents will be saved.

Some of the commonly used options for the `gnatprep` command are:

- `-D`: Define a symbol with a specific value (e.g. `-DNAME=Ada`).
- `-U`: Undefine a symbol (e.g. `-UDEBUG`).
- `-I`: Add an include path for the template file (e.g. `-I/templates`).
- `-C`: Change the comment marker to a specified character (e.g. `-C%`).

The template files can contain placeholders enclosed in `@` symbols that will be replaced by their corresponding values during the preprocessing phase. For example, if the template file contains the placeholder `@NAME@`, it will be replaced by the actual value of `NAME` defined using the `-D` option.

In summary, the `gnatprep` command is a useful tool for generating configuration files or code templates with ease by performing text substitution based on predefined rules and symbols. 

## tldr 
 
> Preprocessor for Ada source code files (part of the GNAT toolchain).
> More information: <https://gcc.gnu.org/onlinedocs/gnat_ugn/Preprocessing-with-gnatprep.html>.

- Use symbol definitions from a file:

`gnatprep {{source_file}} {{target_file}} {{definitions_file}}`

- Specify symbol values in the command line:

`gnatprep -D{{name}}={{value}} {{source_file}} {{target_file}}`
