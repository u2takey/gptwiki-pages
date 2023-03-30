# tokei 
## chatgpt 
Tokei is a command-line tool that provides a summary of code statistics for different programming languages. It can analyze code files in a directory and displays the number of lines, code files, and comments in a table format. 

Here's an example of how to use tokei:

1. Open up your command prompt or terminal on your computer.
2. Navigate to the directory containing the code files you want to analyze. 
3. Type the command "tokei" followed by the options you want to use. For example, "tokei --exclude "*.txt"" would exclude all files with the .txt extension from the analysis. 
4. After running the command, tokei will display a table summarizing the statistics for each programming language used in the code, including the number of lines, files, and comments. 

Tokei is a useful tool for programmers, project managers, and other stakeholders who need to keep track of code statistics and ensure compliance with coding standards. By using tokei, they can quickly get an overview of the amount and complexity of the code, which can help with project planning, resource allocation, and code reviews. 

## tldr 
 
> A program that prints out statistics about code.
> More information: <https://github.com/XAMPPRocky/tokei>.

- Get a report on the code in a directory and all subdirectories:

`tokei {{path/to/directory}}`

- Get a report for a directory excluding `.min.js` files:

`tokei {{path/to/directory}} -e {{*.min.js}}`

- Print out statistics for individual files in a directory:

`tokei {{path/to/directory}} --files`

- Get a report for all files of type Rust and Markdown:

`tokei {{path/to/directory}} -t={{Rust}},{{Markdown}}`
