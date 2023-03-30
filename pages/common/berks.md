# berks 
## chatgpt 
Berks is a command in Chef that is used to manage dependencies in your infrastructure automation code. It is used to gather and resolve cookbook dependencies specified in the Berksfile, which is similar to the Gemfile in Ruby. 

The command `berks` can be used to perform several actions, including:

1. `berks install`: This command reads the Berksfile and installs all the dependencies specified in it. It will also resolve any conflicts if there are multiple versions of a cookbook specified in different dependencies. 

2. `berks upload`: This command uploads a cookbook and its dependencies to a Chef server, making it available for use in the Chef environment. 

3. `berks package`: This command packages a cookbook and its dependencies into a single tarball, which can then be distributed and installed on other machines without an internet connection.

4. `berks update`: This command updates the dependencies in the Berksfile to their latest versions, resolving any conflicts along the way.

Overall, `berks` is a powerful command that simplifies the process of managing cookbook dependencies in large-scale infrastructure automation projects. 

## tldr 
 
> Chef cookbook dependency manager.
> More information: <https://docs.chef.io/berkshelf.html>.

- Install cookbook dependencies into a local repo:

`berks install`

- Update a specific cookbook and its dependencies:

`berks update {{cookbook}}`

- Upload a cookbook to the Chef server:

`berks upload {{cookbook}}`

- View the dependencies of a cookbook:

`berks contingent {{cookbook}}`
