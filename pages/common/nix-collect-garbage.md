# nix-collect-garbage 
## chatgpt 
The command "nix-collect-garbage" is a built-in utility command in the Nix package manager used for cleaning the Nix store by removing all the unused dependencies. In detail, it performs the following actions:

1. It scans the entire Nix store to identify and mark all the valid entries i.e., the packages that are being used by the system or its dependencies.

2. It then removes all the invalid entries i.e., the packages that are not being used by the system or its dependencies. These invalid entries can be in the form of old versions of packages, partially downloaded packages, or packages that were installed but are no longer needed.

3. It then reclaims the disk space occupied by the removed packages from step 2, thereby freeing up valuable disk space.

The "nix-collect-garbage" command is used to clean up the Nix store periodically or after installing/uninstalling packages. It helps to optimize the performance and stability of the system by removing unused dependencies, and it ensures that only the required packages are present in the Nix store. 

## tldr 
 
> Delete unused and unreachable nix store paths.
> Generations can be listed using `nix-env --list-generations`.
> More information: <https://nixos.org/releases/nix/latest/manual/#sec-nix-collect-garbage>.

- Delete all store paths unused by current generations of each profile:

`sudo nix-collect-garbage --delete-old`

- Simulate the deletion of old store paths:

`sudo nix-collect-garbage --delete-old --dry-run`

- Delete all store paths older than 30 days:

`sudo nix-collect-garbage --delete-older-than 30d`
