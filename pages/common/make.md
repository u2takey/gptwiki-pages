# make 
## chatgpt 
The "make" command is a popular build automation tool that is used to automate the process of building software. It is a command-line tool that is commonly used on Linux and other Unix-like operating systems.

When you run the "make" command in a particular directory, it searches for a file called Makefile in that directory. A Makefile is a file that contains a set of instructions (called "rules") for building a software project. These rules define the dependencies between the various components of the project and the steps needed to build and link them together.

The Makefile is typically written in a special syntax known as "makefile syntax". This syntax is used to define targets, dependencies, and recipes for building software.

When the "make" command is run, it first reads the Makefile and determines which targets need to be built. It then checks the dependencies for each target and determines the order in which each dependency needs to be built. Finally, it executes the recipes for each target, which typically involve compiling source code, linking object files, and generating executable files.

Overall, the "make" command is a powerful tool that allows developers to automate the process of building software, saving time and reducing errors in the process. 

## tldr 
 
> Task runner for targets described in Makefile.
> Mostly used to control the compilation of an executable from source code.
> More information: <https://www.gnu.org/software/make/manual/make.html>.

- Call the first target specified in the Makefile (usually named "all"):

`make`

- Call a specific target:

`make {{target}}`

- Call a specific target, executing 4 jobs at a time in parallel:

`make -j{{4}} {{target}}`

- Use a specific Makefile:

`make --file {{path/to/file}}`

- Execute make from another directory:

`make --directory {{path/to/directory}}`

- Force making of a target, even if source files are unchanged:

`make --always-make {{target}}`

- Override a variable defined in the Makefile:

`make {{target}} {{variable}}={{new_value}}`

- Override variables defined in the Makefile by the environment:

`make --environment-overrides {{target}}`
