# nix-build 
## chatgpt 
The "nix-build" command is a command-line tool used with the Nix package manager. It is used to build and generate the output of a Nix expression, which is a declarative configuration file used to specify a set of packages and their dependencies.

When the "nix-build" command is executed, it looks for a file called "default.nix" in the current directory or the path specified as an argument to the command. It then evaluates the expressions in the file and builds the package(s) specified in the expression. The command generates a "result" symlink in the same directory as the "default.nix" file, which points to the output of the build process.

The "nix-build" command supports a variety of options, including the ability to specify a different output directory, specify build arguments, and specify build targets. The command can also be used with the "-A" flag to build a specific attribute of a Nix expression.

Overall, the "nix-build" command is a powerful tool for building and managing packages with the Nix package manager, and is an essential tool for anyone working with Nix-based environments. 

## tldr 
 
> Build a Nix expression.
> More information: <https://nixos.org/releases/nix/latest/manual#sec-nix-build>.

- Build a Nix expression:

`nix-build '<nixpkgs>' --attr {{firefox}}`

- Build a sandboxed Nix expression (on non-NixOS):

`nix-build '<nixpkgs>' --attr {{firefox}} --option sandbox true`
