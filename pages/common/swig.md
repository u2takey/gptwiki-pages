# swig 
## chatgpt 
SWIG (Simplified Wrapper and Interface Generator) is a software development tool that is used to connect software written in various programming languages to C and C++ programming languages. It generates code automatically that allows different programming languages to interact with each other using the C and C++ programming languages. SWIG supports many popular programming languages, including Python, Java, Ruby, Perl, Tcl, and PHP.

The swig command is used to generate wrapper code that makes it easy to interface C and C++ code with the various supported programming languages. The command takes input files, which typically include a header file containing function and data declarations, as well as a SWIG interface file, which specifies the mapping between the C/C++ code and the target programming language. The output is a set of wrapper files and a target language module file, which is then compiled with the target language's compiler.

The command has many options that allow developers to customize the output code, including flags to specify the target language, output directory, and optimization level. Additionally, SWIG provides a range of tools and libraries to help developers work with the generated output. Overall, swig is a powerful tool that helps developers create seamless and efficient interfaces between different programming languages. 

## tldr 
 
> Generate bindings between C / C++ code and various high level languages such as JavaScript, Python, C#, and more.
> It uses special .i or .swg files to generate the bindings (C/C++ with SWIG directives, then outputs a C/C++ file that contains all the wrapper code needed to build an extension module.
> More information: <http://www.swig.org>.

- Generate a binding between C++ and Python:

`swig -c++ -python -o {{path/to/output_wrapper.cpp}} {{path/to/swig_file.i}}`

- Generate a binding between C++ and Go:

`swig -go -cgo -intgosize 64 -c++ {{path/to/swig_file.i}}`

- Generate a binding between C and Java:

`swig -java {{path/to/swig_file.i}}`

- Generate a binding between C and Ruby and prefix the Ruby module with {{foo::bar::}}:

`swig -ruby -prefix "{{foo::bar::}}" {{path/to/swig_file.i}}`
