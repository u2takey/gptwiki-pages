# gdebi 
## chatgpt 
gdebi is a command-line utility used in Debian-based Linux distributions to install .deb packages with their dependencies. The gdebi tool is different from other package installation tools like apt-get because it enables users to download and install a package with its dependencies in a single command.

The syntax for gdebi command is:

``` gdebi [package_name].deb ```

Here, the [package_name] argument should be replaced with the name of the package that you want to install. The .deb file should be located in the directory from which you are running the command.

When you run the gdebi command, it checks whether all the dependencies for the package are available on your system. If any are missing, it will prompt you to install them. Once all dependencies are met, it will ask you to confirm the installation by typing 'y.'

In summary, the gdebi command is used to install a .deb package with its dependencies in a single command. It is a useful tool for users who want to easily install packages in Debian-based Linux distributions without worrying about dependencies. 

## tldr 
 
> Simple tool to install `.deb` files.
> More information: <https://www.commandlinux.com/man-page/man1/gdebi.1.html>.

- Install local `.deb` packages resolving and installing its dependencies:

`gdebi {{path/to/package.deb}}`

- Display the program version:

`gdebi --version`

- Do not show progress information:

`gdebi {{path/to/package.deb}} --quiet`

- Set an APT configuration option:

`gdebi {{path/to/package.deb}} --option={{APT_OPTS}}`

- Use alternative root dir:

`gdebi {{path/to/package.deb}} --root={{path/to/root_dir}}`
