# slimrb 
## chatgpt 
The command `slimrb` is used to compile or transform Slim markup files into HTML format. Slim is a template engine that allows developers to write HTML code in a more concise and readable format.

When you run `slimrb`, it parses the Slim code and renders it as HTML. The output is sent to the standard output stream or can be directed to a file.

Here are the basic steps involved in using the `slimrb` command:

1. Create a Slim file with the extension `.slim`.
2. Open terminal or command prompt.
3. Navigate to the directory containing the Slim file.
4. Type `slimrb filename.slim` and hit enter.
5. The command will parse and render the Slim into HTML format and output it to the terminal.

The `slimrb` command can also accept several options to modify the output of the Slim file. For example, you can use the `-p` option to pretty print the HTML output or the `-r` option to require a specific Ruby library file.

Overall, the `slimrb` command is a useful tool for developers using the Slim template engine, as it allows them to easily transform their code into readable and optimized HTML pages. 

## tldr 
 
> Convert Slim files to HTML.
> More information: <https://rdoc.info/gems/slim/frames#slim-command-slimrb>.

- Convert a Slim file to HTML:

`slimrb {{input.slim}} {{output.html}}`

- Convert a Slim file and output to prettified HTML:

`slimrb --pretty {{input.slim}} {{output.html}}`

- Convert a Slim file to ERB:

`slimrb --erb {{input.slim}} {{output.erb}}`
