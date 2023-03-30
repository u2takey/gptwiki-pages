# fossil init 
## chatgpt 
Fossil is a distributed version control system that allows you to track changes to files over time. The "fossil init" command is used to create a new Fossil repository. When you run this command, Fossil will create a new repository with an empty "master" branch. Here's what happens when you run the "fossil init" command:

1. Fossil creates a new directory to hold the repository. This directory can be named whatever you want, but it's typically called "myproject.fossil".

2. Fossil creates a new repository database file called "myproject.fossil".

3. Fossil initializes the repository with an empty "master" branch.

4. Fossil creates some default settings for the repository.

Once the repository is initialized, you can start adding files and making changes to them. You can also create new branches, merge branches, and perform other operations using the Fossil command-line tools. 

## tldr 
 
> Initialize a new repository for a project.
> See also: `fossil clone`.
> More information: <https://fossil-scm.org/home/help/init>.

- Create a new repository in a named file:

`fossil init {{path/to/filename}}`
