# code 
## chatgpt 
The term "code" is not a specific command, but rather a generic term for a set of programming instructions that is written in a particular language. 

In general, a "code" refers to a block of computer programming instructions that tell a computer or other device how to perform a specific task or solve a certain problem. Programmers use coding languages like Java, Python, C++, and many others to write these instructions in a format that the computer can read and execute.

When someone refers to "writing code", they mean creating or editing a set of programming instructions for a specific purpose, which could range from creating complex software applications to developing simple scripts to automate repetitive tasks. The process of coding requires knowledge of specific programming languages, syntax, and best practices in order to produce efficient, functional code that meets the desired outcomes. 

## tldr 
 
> Cross platform and extensible code editor.
> More information: <https://github.com/microsoft/vscode>.

- Start Visual Studio Code:

`code`

- Open specific files/directories:

`code {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Compare two specific files:

`code --diff {{path/to/file1}} {{path/to/file2}}`

- Open specific files/directories in a new window:

`code --new-window {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Install/uninstall a specific extension:

`code --{{install|uninstall}}-extension {{publisher.extension}}`

- Print installed extensions:

`code --list-extensions`

- Print installed extensions with their versions:

`code --list-extensions --show-versions`

- Start the editor as a superuser (root) while storing user data in a specific directory:

`sudo code --user-data-dir {{path/to/directory}}`
