# vswhere 
## chatgpt 
Vswhere is a command-line utility that is used to locate and retrieve information about the installed Visual Studio instances on a computer. It can be used to query all installed versions of Visual Studio, including the latest version, and to retrieve information such as the installation location, product name, version, edition, and the installed components.

The vswhere command can be used to perform a variety of actions including:

- Querying for the latest installed version of Visual Studio using the "latest" option.
- Listing all installed instances of Visual Studio using the "all" option.
- Retrieving specific information about a particular Visual Studio instance using command-line switches such as "-property" to retrieve an instance property, or "-products" to retrieve a list of installed products.

Some common examples of using the vswhere command are:

- Find the latest installation directory of Visual Studio:
   vswhere -latest -property installationPath

- List all installed Visual Studio instances:
   vswhere -all

- Retrieve information about a specific Visual Studio edition:
  vswhere -products Microsoft.VisualStudio.Community -version [version number] -property displayName

The vswhere command is a useful tool for developers looking to automate certain installation and configuration tasks, and for administrators who need to manage multiple instances of Visual Studio on a computer or network. 

## tldr 
 
> Locate Visual Studio 2017 and newer installations.
> More information: <https://github.com/microsoft/vswhere>.

- Find the path of vcvarsall.bat to set environment variables:

`vswhere -products * -latest -prerelease -find **\VC\Auxiliary\Build\vcvarsall.bat`

- Find the directory of the x64 MSVC compiler (cl.exe, etc):

`vswhere -products * -latest -prerelease -find **\Hostx64\x64\*`

- Find the directory of Clang bundled with Visual Studio bundled (clang-cl, clang-tidy, etc):

`vswhere -products * -latest -prerelease -find **\Llvm\bin\*`

- Find the path of `MSBuild.exe`:

`vswhere -products * -latest -prerelease -find MSBuild\**\Bin\MSBuild.exe`
