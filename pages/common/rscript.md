# Rscript 
## chatgpt 
Rscript is a command-line interface executable program that allows users to run and execute R scripts without opening R environment on the terminal. The Rscript command is used to execute an R script from the command-line interface. 

The syntax for Rscript is:

Rscript [options] filename [arguments]

Where:
- [options]: Optional command-line arguments that modify the behavior of Rscript. These can include options like specifying a working directory or setting output file names.
- filename: The name of the R script file that contains the code to be executed.
- [arguments]: Optional arguments that can be passed to the R script to be used as input parameters.

For example, to execute a simple R script called "my_script.R" with no arguments, the command would be:

Rscript my_script.R

If the script requires an argument to be passed, the command would be:

Rscript my_script.R argument1 argument2

Rscript can also be used in combination with other command-line tools such as piping data to and from the R script or calling R functions from other programming languages. 

## tldr 
 
> Run a script with the R programming language.
> More information: <https://www.r-project.org>.

- Run a script:

`Rscript {{path/to/file.R}}`

- Run a script in vanilla mode (i.e. a blank session that doesn't save the workspace at the end):

`Rscript --vanilla {{path/to/file.R}}`

- Execute one or more R expressions:

`Rscript -e {{expression1}} -e {{expression2}}`

- Display R version:

`Rscript --version`
