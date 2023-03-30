# rails routes 
## chatgpt 
The command "rails routes" is used in Ruby on Rails web application development to generate a list of all the defined routes in the application. 

When the command is executed in the command line, it will show a table of all the routes for the different HTTP requests (GET, POST, PUT, DELETE) along with the controller and action they are mapped to. 

The table provides a quick overview of all the routes that are available in the application, including their names, paths, and HTTP verbs. This command can be particularly helpful for debugging routing issues and ensuring that all the routes are correctly defined and mapped to their respective controllers and actions. 

Additionally, there are a number of helpful options that can be used with the "rails routes" command, including filtering the routes by controller, action, or path, and formatting the output for better readability. 

## tldr 
 
> List routes in a Rails application.
> More information: <https://guides.rubyonrails.org/routing.html>.

- List all routes:

`rails routes`

- List all routes in an expanded format:

`rails routes --expanded`

- List routes partially matching URL helper method name, HTTP verb, or URL path:

`rails routes -g {{posts_path|GET|/posts}}`

- List routes that map to a specified controller:

`rails routes -c {{posts|Posts|Blogs::PostsController}}`
