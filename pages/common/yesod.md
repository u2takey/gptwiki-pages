# yesod 
## chatgpt 
Yesod is a web framework in the Haskell language. It is designed to help developers create high-performance web applications quickly and easily. The "yesod" command is a command-line interface (CLI) tool that you can use to create and manage Yesod projects.

Here are some of the basic commands that you can use with "yesod":

- `yesod init` - This command initializes a new Yesod project. It creates a basic project layout with all the necessary files and directories.

- `yesod devel` - This command starts a development server that serves your Yesod application. This server will automatically reload your application when you make changes to the code, making it easy to experiment and iterate quickly.

- `yesod test` - This command runs the tests for your Yesod application. You can write tests in Haskell using popular testing frameworks like HUnit or QuickCheck.

- `yesod deploy` - This command deploys your Yesod application to a production environment. You can use this command to build your application and package it up for deployment to a web server or cloud hosting provider.

Overall, the "yesod" command is an essential tool for developing and managing Yesod web applications. It provides a streamlined workflow for creating, testing, and deploying your code, helping you to build robust and scalable web applications with ease. 

## tldr 
 
> Helper tool for Yesod, a Haskell-based web framework.
> All Yesod commands are invoked through the `stack` project manager.
> More information: <https://github.com/yesodweb/yesod>.

- Create a new scaffolded site, with SQLite as backend, in the `my-project` directory:

`stack new {{my-project}} {{yesod-sqlite}}`

- Install the Yesod CLI tool within a Yesod scaffolded site:

`stack build yesod-bin cabal-install --install-ghc`

- Start development server:

`stack exec -- yesod devel`

- Touch files with altered Template Haskell dependencies:

`stack exec -- yesod touch`

- Deploy application using Keter (Yesod's deployment manager):

`stack exec -- yesod keter`
