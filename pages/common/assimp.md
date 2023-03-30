# assimp 
## chatgpt 
Assimp is a command-line tool that allows you to process 3D models in various formats. 

Here are a few examples of how to use the `assimp` command:

1. To get information about a 3D model:

`assimp info model.obj`

This will display information such as the number of vertices, faces, materials used, etc.

2. To convert a 3D model from one format to another:

`assimp export model.obj model.fbx`

This will convert the model from OBJ format to FBX format.

3. To extract specific parts of a 3D model:

`assimp export -skeleton model.fbx model.skel`

This will extract the skeleton data from the FBX file and save it as a new file.

4. To merge multiple 3D models into a single file:

`assimp export -merge model1.obj model2.fbx mergedModel.fbx`

This will merge the two models into a single FBX file.

Overall, the `assimp` command provides a lot of functionality for working with 3D models, which makes it a useful tool for game developers, animators, and other professionals in the field of 3D graphics. 

## tldr 
 
> Command-line client for the Open Asset Import Library.
> Supports loading of 40+ 3D file formats, and exporting to several popular 3D formats.
> More information: <http://www.assimp.org/>.

- List all supported import formats:

`assimp listext`

- List all supported export formats:

`assimp listexport`

- Convert a file to one of the supported output formats, using the default parameters:

`assimp export {{input_file.stl}} {{output_file.obj}}`

- Convert a file using custom parameters (the dox_cmd.h file in assimp's source code lists available parameters):

`assimp export {{input_file.stl}} {{output_file.obj}} {{parameters}}`

- Display a summary of a 3D file's contents:

`assimp info {{path/to/file}}`

- List all supported subcommands ("verbs"):

`assimp help`

- Get help on a specific subcommand (e.g. the parameters specific to it):

`assimp {{subcommand}} --help`
