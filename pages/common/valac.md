# valac 
## chatgpt 
The command "valac" is a compiler for the Vala programming language. Vala is a programming language that is designed to be a modern programming language that compiles into efficient, native code. The Vala language has syntax similar to C#, Java or Swift, but it compiles into C code that can be compiled into efficient native code.

To use the "valac" command, you need to have the Vala programming language installed on your computer. Once you have installed Vala, you can open your terminal or command prompt, and run the "valac" command followed by the name of the Vala source code file that you want to compile. 

The "valac" command has several options that you can use to control the compilation process, such as specifying the output file name, defining compiler flags, or enabling debugging or optimization. You can use the "--help" option to see a list of all available options.

After you run the "valac" command, it will generate a binary executable file that you can run on your system. The generated binary file will contain native code that can be executed by your system's processor. This allows Vala programs to have excellent performance and memory efficiency. 

## tldr 
 
> Vala code compiler.
> Tutorial: <https://wiki.gnome.org/Projects/Vala/Tutorial>.
> More information: <https://valadoc.org/>.

- Compile a vala file, with gtk+:

`valac {{path/to/file.vala}} --pkg {{gtk+-3.0}}`

- Display version info:

`valac --version`

- Display helper message:

`valac --help`
