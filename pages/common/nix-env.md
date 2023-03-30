# nix-env 
## chatgpt 
nix-env is a command line tool that is used in NixOS, a Linux distribution, to manage packages and environments. 

Here are the details of nix-env command:

Usage: 

nix-env [OPTIONS] SUBCOMMAND [ARGS...]

Options:

- -q, --query: Show the list of installed packages along with their paths.
- -i, --install: Installs a package or a set of packages.
- -e, --uninstall: Uninstalls a package or a set of packages.
- -u, --update: Updates all installed packages.
- -p, --profile: Specifies the profile to be used for installing packages.
- -S, --switch: Sets the active profile and creates a symlink to the profile directory.
- -f, --file: Specifies the path to the package set to install as a profile.

Subcommands:

- list: Shows the list of available packages to install.
- info: Shows information about a specific package.
- install: Installs a package or a set of packages.
- uninstall: Uninstalls a package or a set of packages.
- upgrade: Upgrades a package or a set of packages.

Overall, nix-env is a very powerful and flexible tool that allows users to manage their packages and environments easily in a reproducible and consistent manner. 

## tldr 
 
> Manipulate or query Nix user environments.
> More information: <https://nixos.org/manual/nix/stable/#sec-nix-env>.

- List all installed packages:

`nix-env -q`

- Query installed packages:

`nix-env -q {{search_term}}`

- Query available packages:

`nix-env -qa {{search_term}}`

- Install package:

`nix-env -iA nixpkgs.{{pkg_name}}`

- Install a package from a URL:

`nix-env -i {{pkg_name}} --file {{example.com}}`

- Uninstall package:

`nix-env -e {{pkg_name}}`

- Upgrade one package:

`nix-env -u {{pkg_name}}`

- Upgrade all packages:

`nix-env -u`
