# vue init 
## chatgpt 
The `vue init` command is used in Vue.js to scaffold a new project. When this command is run, Vue.js will prompt for certain configuration options such as project name, author, package manager, CSS preprocessor, etc. Once the user has answered these prompts, Vue.js will generate a new project with the specified configurations.

Here is a breakdown of the different pieces of the `vue init` command:

- `vue`: This is the Vue.js CLI (Command Line Interface) command.
- `init`: This is a sub-command of the Vue.js CLI used to initialize a new project.

When this command is run, Vue.js will create a new project structure containing many folders and files such as `src`, `components`, `router`, `App.vue`, `main.js`, and more.

In summary, the `vue init` command is a quick and easy way to scaffold a new Vue.js project with minimal configuration. 

## tldr 
 
> Legacy project initialization subcommand of the Vue.js framework.
> More information: <https://cli.vuejs.org/guide/creating-a-project.html#pulling-2-x-templates-legacy>.

- Create a new project using one of the default templates:

`vue init {{webpack|webpack-simple|browserify|browserify-simple|simple}} {{project_name}}`

- Create a new project using a local template:

`vue init {{path/to/template_directory}} {{project_name}}`

- Create a new project using a template from GitHub:

`vue init {{username}}/{{repo}} {{project_name}}`
