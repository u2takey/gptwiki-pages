# skopeo 
## chatgpt 
Skopeo is a command line tool for working with remote container image repositories and helps to manage and inspect the container images. Here are some of the commands that can be used with Skopeo:

1. Copy: Allows for copying an image from one registry to another or within the same registry.

Syntax: `skopeo copy [OPTIONS] SRC_URI DEST_URI`

Example: `skopeo copy docker://example.com/foo:latest dir://local/path/foo:latest`

2. Inspect: Displays information about a container image such as its metadata and configuration.

Syntax: `skopeo inspect [OPTIONS] IMAGE_URI`

Example: `skopeo inspect docker://example.com/foo:latest`

3. Delete: Allows for removal of a container image from a registry.

Syntax: `skopeo delete [OPTIONS] IMAGE_URI`

Example: `skopeo delete docker://example.com/foo:latest`

4. Login: Authenticates to a container image registry.

Syntax: `skopeo login [OPTIONS] REGISTRY`

Example: `skopeo login --username myuser --password mypassword example.com`

5. List-tags: Lists the tags available for a container image.

Syntax: `skopeo list-tags [OPTIONS] REGISTRY/IMAGE`

Example: `skopeo list-tags docker://example.com/foo`

These commands can be used to manage container images in a secure and efficient way. 

## tldr 
 
> Container image management toolbox.
> Provides various utility commands to manage remote container images.
> More information: <https://github.com/containers/skopeo>.

- Inspect a remote image from a registry:

`skopeo inspect docker://{{registry_hostname}}/{{image:tag}}`

- List available tags for a remote image:

`skopeo list-tags docker://{{registry_hostname}}/{{image}}`

- Download an image from a registry:

`skopeo copy docker://{{registry_hostname}}/{{image:tag}} dir:{{path/to/directory}}`

- Copy an image from one registry to another:

`skopeo copy docker://{{source_registry}}/{{image:tag}} docker://{{destination_registry}}/{{image:tag}}`

- Delete an image from a registry:

`skopeo delete docker://{{registry_hostname}}/{{image:tag}}`

- Log in to a registry:

`skopeo login --username {{username}} {{registry_hostname}}`
