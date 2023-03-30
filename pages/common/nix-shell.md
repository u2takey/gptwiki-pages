# nix-shell 
## chatgpt 
`nix-shell` is a command that creates a temporary environment with all the dependencies required to run a project or set of scripts. 

When executed without any arguments, `nix-shell` will activate an environment based on the `shell.nix` file present in the current directory. The `shell.nix` file is a declarative specification of the dependencies required for the project, which may include packages, libraries, and system tools. The specifications included in the `shell.nix` file are resolved by the Nix package manager, which ensures that all dependencies are compatible and do not have any conflicts.

The `nix-shell` command sets up an environment that has all the dependencies specified in the `shell.nix` file. It modifies the user's `PATH` variable to include the paths to the required binaries and libraries. This makes it easy to run scripts or programs that depend on these dependencies, without having to worry about installing the dependencies on the host system.

Additionally, `nix-shell` can be used to change the default shell for the current session to the one specified in the `shell.nix` file. This can be accomplished by specifying the `--command` flag and passing in the name of the desired shell, such as `zsh` or `bash`.

Overall, `nix-shell` simplifies the process of managing dependencies for a project and ensures that the required packages and libraries are readily available for development and testing. 

## tldr 
 
> Start an interactive shell based on a Nix expression.
> More information: <https://nixos.org/manual/nix/stable/#sec-nix-shell>.

- Start with nix expression in `shell.nix` or `default.nix` in the current directory:

`nix-shell`

- Run shell command in non-interactive shell and exit:

`nix-shell --run "{{command}} {{arg1 arg2 ...}}"`

- Start with expression in `default.nix` in the current directory:

`nix-shell {{default.nix}}`

- Start with packages loaded from nixpkgs:

`nix-shell --packages {{package_name_1 package_name_2 ...}}`

- Start with packages loaded from specific nixpkgs revision:

`nix-shell --packages {{package_name_1 package_name_2 ...}} -I nixpkgs={{https://github.com/NixOS/nixpkgs/archive/nixpkgs_revision.tar.gz}}`

- Evaluate rest of file in specific interpreter, for use in `#!-scripts` (see <https://nixos.org/manual/nix/stable/#use-as-a-interpreter>):

`nix-shell -i {{interpreter}} --packages {{package_name_1 package_name_2 ...}}`
