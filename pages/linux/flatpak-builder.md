# flatpak-builder 
## chatgpt 
Flatpak-builder is a command-line tool used to build and package Flatpak applications. Flatpak is a Linux-based application packaging and delivery system that allows developers to package an application and its dependencies into a single runtime environment that can be easily deployed on different Linux distributions.

The flatpak-builder command follows a specific format that includes several options and arguments:

`flatpak-builder [options] REPO-DIR REF [APP-DIR]`

- `options`: Optional arguments that modify the behavior of the command.
- `REPO-DIR`: The directory where the Flatpak repository is located. This directory must exist and be writable by the user.
- `REF`: The name of the branch or tag in the source code repository that corresponds to the version of the application being built.
- `APP-DIR`: Optional directory containing the source code for the application. If not specified, flatpak-builder will look for a file called `manifest.json` in the current directory.

Some of the most common options for flatpak-builder include:

- `--force-clean`: Remove any existing build artifacts before starting the build.
- `--ccache`: Use the ccache tool to speed up the build process by caching object files.
- `--repo=<URI>`: Use the specified Flatpak repository as the destination for the built application.

Overall, the flatpak-builder command is a powerful tool that simplifies the process of building and packaging Flatpak applications, making it easier for developers to create cross-distribution software packages. 

## tldr 
 
> Help build application dependencies.
> More information: <https://docs.flatpak.org/en/latest/flatpak-builder-command-reference.html>.

- Build a Flatpak and export it to a new repository:

`flatpak-builder {{path/to/build_directory}} {{path/to/manifest}}`

- Build a Flatpak and export it to the specified repository:

`flatpak-builder --repo={{repository_name}} {{path/to/build_directory}} {{path/to/manifest}}`

- Build a Flatpak and install it locally:

`flatpak-builder --install {{path/to/build_directory}} {{path/to/manifest}}`

- Build and sign a Flatpak and export it to the specified repository:

`flatpak-builder --gpg-sign={{key_id}} --repo={{repository_name}} {{path/to/manifest}}`

- Run a shell inside of an application sandbox without installing it:

`flatpak-builder --run {{path/to/build_directory}} {{path/to/manifest}} {{sh}}`
