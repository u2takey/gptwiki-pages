# sass 
## chatgpt 
Sass is a command-line tool that compiles Sass files (files with .scss or .sass extensions) into CSS files. The Sass command can be used in several ways, including:

1. Sass watch: This command watches a directory and compiles Sass files whenever they change. To use Sass watch, navigate to the directory containing your Sass files and run the command "sass --watch input.scss:output.css". This will compile the input.scss file into output.css whenever input.scss is updated.

2. Sass compile: This command compiles a single Sass file into a CSS file. To use Sass compile, navigate to the directory containing your Sass file and run the command "sass input.scss output.css". This will compile the input.scss file into output.css.

3. Sass interactive shell: This command opens an interactive shell that allows you to experiment with Sass. To use Sass interactive shell, run the command "sass --interactive". This will open the interactive shell where you can type Sass commands and see the output. 

Overall, the Sass command is used to compile Sass files into CSS files, and provides several options to watch or compile files. It is a useful tool for developers who want to simplify their CSS workflow and take advantage of the features offered by Sass. 

## tldr 
 
> Converts SCSS or Sass files to CSS.
> More information: <https://sass-lang.com/documentation/cli/dart-sass>.

- Convert a SCSS or Sass file to CSS and print out the result:

`sass {{inputfile.scss|inputfile.sass}}`

- Convert a SCSS or Sass file to CSS and save the result to a file:

`sass {{inputfile.scss|inputfile.sass}} {{outputfile.css}}`

- Watch a SCSS or Sass file for changes and output or update the CSS file with same filename:

`sass --watch {{inputfile.scss|inputfile.sass}}`

- Watch a SCSS or Sass file for changes and output or update the CSS file with the given filename:

`sass --watch {{inputfile.scss|inputfile.sass}}:{{outputfile.css}}`
