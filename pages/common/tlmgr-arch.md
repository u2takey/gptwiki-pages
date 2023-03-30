# tlmgr arch 
## chatgpt 
The `tlmgr arch` command is used in TeX Live Manager (tlmgr) to display the architecture of the TeX Live distribution that is currently installed on the system. 

An architecture in TeX Live refers to the CPU and operating system for which the TeX binaries are compiled. The different architectures that TeX Live supports include:

- `x86_64-linux`: 64-bit Linux
- `i386-linux`: 32-bit Linux
- `win32`: 32-bit Windows
- `x86_64-darwin`: 64-bit macOS
- `universal-darwin`: Universal macOS (both 32-bit and 64-bit)

When you run the `tlmgr arch` command, it will output the current architecture of the TeX Live installation, such as `x86_64-linux` or `x86_64-darwin`. 

Knowing the architecture of your TeX Live distribution is important when installing and managing packages and updating your TeX installation, as different architectures may require different packages or updates. 

## tldr 
 
> This command is an alias of `tlmgr platform`.
> More information: <https://www.tug.org/texlive/tlmgr.html>.

- View documentation for the original command:

`tldr tlmgr platform`
