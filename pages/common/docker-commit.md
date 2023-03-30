# docker commit 
## chatgpt 
The `docker commit` command is used to create a new image from a container that has been modified. This new image can then be used to create new containers with the modified state.

The basic syntax of the command is:

```
$ docker commit [OPTIONS] CONTAINER [REPOSITORY[:TAG]]
```

Where:

- `OPTIONS`: Optional parameters such as `-a` to specify the author of the new image or `-m` to add a commit message.
- `CONTAINER`: The name or ID of the container to be committed.
- `REPOSITORY`: The name of the repository to use for the new image.
- `TAG`: An optional tag for the new image.

When the command is run, Docker takes a snapshot of the container and creates a new image from it. The new image is tagged with the name and tag specified and can then be pushed to a registry for others to use or pulled down to another machine.

It's important to note that the `docker commit` command should be used sparingly and only in cases where it's necessary to modify an existing container. It's generally recommended to use a Dockerfile to create new images in a more reproducible and maintainable way. 

## tldr 
 
> Create a new image from a container’s changes.
> More information: <https://docs.docker.com/engine/reference/commandline/commit/>.

- Create an image from a specific container:

`docker commit {{container}} {{image}}:{{tag}}`

- Apply a `CMD` Dockerfile instruction to the created image:

`docker commit --change="CMD {{command}}" {{container}} {{image}}:{{tag}}`

- Apply an `ENV` Dockerfile instruction to the created image:

`docker commit --change="ENV {{name}}={{value}}" {{container}} {{image}}:{{tag}}`

- Create an image with a specific author in the metadata:

`docker commit --author="{{author}}" {{container}} {{image}}:{{tag}}`

- Create an image with a specific comment in the metadata:

`docker commit --message="{{comment}}" {{container}} {{image}}:{{tag}}`

- Create an image without pausing the container during commit:

`docker commit --pause={{false}} {{container}} {{image}}:{{tag}}`

- Display help:

`docker commit --help`
