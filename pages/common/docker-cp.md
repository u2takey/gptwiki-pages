# docker cp 
## chatgpt 
The `docker cp` command is used to copy files or directories between a container and the host system. The syntax of the command is as follows:

```
docker cp [OPTIONS] CONTAINER:SRC_PATH DEST_PATH
docker cp [OPTIONS] SRC_PATH|CONTAINER:SRC_PATH DEST_PATH
```

Here are the different components of this command:

- `OPTIONS`: Optional flags that modify the behavior of the command. Some of the commonly used options include `-a` (preserve file ownership and permissions), `-L` (follow symbolic links), and `--help` (show help message).
- `CONTAINER`: The name or ID of the container from/to which files or directories need to be copied.
- `SRC_PATH`: The full path of the file or directory inside the container that needs to be copied.
- `DEST_PATH`: The full path of the file or directory on the host system where the copied files or directories will be saved.

The `docker cp` command is useful for transferring files between the host system and the container, especially when the `docker cp` command is the most direct method of communication between host and container. Additionally, you may want to inspect or manipulate a file in a container, and you'll want to take it out of the container to work with. 

Keep in mind that the `docker cp` command can only copy files to or from a container that is running. If you need to copy files to or from a container that is not running, you'll need to use a different approach such as creating a new container and mounting volumes between the two. 

## tldr 
 
> Copy files or directories between host and container filesystems.
> More information: <https://docs.docker.com/engine/reference/commandline/cp>.

- Copy a file or directory from the host to a container:

`docker cp {{path/to/file_or_directory_on_host}} {{container_name}}:{{path/to/file_or_directory_in_container}}`

- Copy a file or directory from a container to the host:

`docker cp {{container_name}}:{{path/to/file_or_directory_in_container}} {{path/to/file_or_directory_on_host}}`

- Copy a file or directory from the host to a container, following symlinks (copies the symlinked files directly, not the symlinks themselves):

`docker cp --follow-link {{path/to/symlink_on_host}} {{container_name}}:{{path/to/file_or_directory_in_container}}`
