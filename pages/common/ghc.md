# ghc 
## chatgpt 
ghc is a command that invokes the Glasgow Haskell Compiler (GHC), which is a compiler for the Haskell programming language. Haskell is a functional programming language that is designed to be declarative, which means that you specify what you want the program to do, rather than how to do it. GHC translates Haskell code into machine code that can be run on a variety of platforms, including Windows, macOS, and Linux.

When you run the ghc command, you typically pass it one or more source code files that contain Haskell code that you want to compile. For example, you might run the following command to compile a file named MyProgram.hs:

```
ghc MyProgram.hs
```

The GHC compiler will then parse the Haskell code in the file, type check it to ensure that it is well-formed, and generate object code that can be executed. The resulting executable will be placed in the same directory as the source file, and will have the same name with the addition of an extension that is specific to the platform. For example, on Windows the resulting executable might be named MyProgram.exe, while on macOS it might be named MyProgram.app.

In addition to simply compiling Haskell code, the ghc command supports a variety of options and flags that can be used to customize the compilation process. For example, you might use an option like -O2 to enable aggressive optimization, or -static to statically link any necessary libraries. There are many options available, and you can find a complete list in the GHC documentation. 

## tldr 
 
> The Glasgow Haskell Compiler.
> Compiles and links Haskell source files.
> More information: <https://www.haskell.org/ghc>.

- Find and compile all modules in the current directory:

`ghc Main`

- Compile a single file:

`ghc {{file.hs}}`

- Compile using extra optimization:

`ghc -O {{file.hs}}`

- Stop compilation after generating object files (.o):

`ghc -c {{file.hs}}`

- Start a REPL (interactive shell):

`ghci`

- Evaluate a single expression:

`ghc -e {{expression}}`
