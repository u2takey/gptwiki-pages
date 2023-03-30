# skaffold 
## chatgpt 
Skaffold is a popular and powerful command-line tool used to automate the continuous development and deployment process of Kubernetes applications. It enables developers to define their resource requirements in a YAML configuration file, which specifies which services and applications to build, test, and deploy, and how to do so.

The skaffold command provides several sub-commands that help developers manage and streamline their Kubernetes development workflow. These sub-commands include:

- `init`: This command initializes a new Skaffold configuration file based on the language and framework of the project.
- `build`: This command builds the Docker images for the specified services and applications in the Skaffold configuration file.
- `test`: This command runs the tests for the specified services and applications in the Skaffold configuration file.
- `deploy`: This command deploys the built images to the Kubernetes cluster.
- `dev`: This command watches the local file system for changes and automatically rebuilds, tests, and deploys the application to the Kubernetes cluster as changes are made.

Skaffold has a rich set of features that simplify the build and deployment process, including support for incremental builds, live reloading, and caching of Docker images, as well as automated cleanup of resources. Skaffold is also extensible through the use of plugins, which can be used to add additional functionality or integrate with other tools or services. 

## tldr 
 
> A tool that facilitates continuous development for Kubernetes applications.
> More information: <https://skaffold.dev>.

- Build the artifacts:

`skaffold build -f {{skaffold.yaml}}`

- Build and deploy your app every time your code changes:

`skaffold dev -f {{skaffold.yaml}}`

- Run a pipeline file:

`skaffold run -f {{skaffold.yaml}}`

- Run a diagnostic on Skaffold:

`skaffold diagnose -f {{skaffold.yaml}}`

- Deploy the artifacts:

`skaffold deploy -f {{skaffold.yaml}}`
