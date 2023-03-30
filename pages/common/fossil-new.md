# fossil new 
## chatgpt 
The `fossil new` command is used to create a new Fossil repository. 

When the command is executed, it prompts the user to enter certain details to configure the new repository, including the name of the repository file, description of the project, and the name of the initial branch. 

For example, to create a new repository called "myproject" with the description "A test project" and the initial branch called "dev", the command would be:

```
fossil new myproject.fossil --description "A test project" --branch dev
```

The above command creates a new file called "myproject.fossil" in the current directory, and initializes it as a new Fossil repository with the specified details.

Once the repository is created, it can be used to store project files, track changes, manage tickets, and collaborate with other developers using Fossil's built-in capabilities. 

## tldr 
 
> This command is an alias of `fossil init`.
> More information: <https://fossil-scm.org/home/help/new>.

- View documentation for the original command:

`tldr fossil-init`
