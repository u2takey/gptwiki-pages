# vala 
## chatgpt 
Vala is not a command, but a programming language. It is an object-oriented programming language that is syntactically similar to C# and is designed to bring modern programming concepts to the Linux desktop.

Vala combines the efficiency and low-level control of C with high-level features such as garbage collection, type safety, and memory management using reference counting.  It is designed to target the GObject system in the GNOME desktop environment, which allows for easy integration with existing applications.

To use Vala, you will typically write your code in a text editor and save it with a .vala file extension. You can then compile your code using the valac compiler, which generates C code that can be linked with other libraries and executed as a binary.

Vala is a popular choice for developing desktop applications on Linux, as well as for system programming tasks such as writing daemons and plugins. It has a growing community of developers and is actively maintained and updated, making it a reliable choice for building Linux-based software. 

## tldr 
 
> Vala code runner.
> Tutorial: <https://wiki.gnome.org/Projects/Vala/Tutorial>.
> More information: <https://valadoc.org/>.

- Run a vala file, with gtk+:

`vala {{path/to/file.vala}} --pkg {{gtk+-3.0}}`

- Display version info:

`vala --version`

- Display helper message:

`vala --help`
