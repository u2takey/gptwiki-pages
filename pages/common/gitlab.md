# gitlab 
## chatgpt 
As an AI language model, I don't have personal experience of using GitLab, but I can provide you with an explanation of the command in general. 

GitLab is a web-based Git repository manager that provides features for continuous integration, code deployment, and collaboration. When you run the command `gitlab`, it depends on the context of where and how you use it.

If you use the command in a terminal or command-line interface (CLI), it may refer to the GitLab CLI, which is a tool for interacting with GitLab repositories and projects through a text-based interface. With the GitLab CLI, you can manage issues, merge requests, repositories, and user accounts.

Alternatively, if you use the `gitlab` command in a Git-enabled project directory, it may refer to the remote GitLab repository that your local Git repository is connected to. For example, `gitlab push` is a command for pushing changes from your local repository to the GitLab remote repository.

In summary, the `gitlab` command depends on the context in which it is used. It may refer to the GitLab CLI tool, the GitLab remote repository, or other GitLab-related commands and functionalities. 

## tldr 
 
> Ruby wrapper and CLI for the GitLab API.
> Some subcommands such as `gitlab ctl` have their own usage documentation.
> More information: <https://narkoz.github.io/gitlab/>.

- Create a new project:

`gitlab create_project {{project_name}}`

- Get info about a specific commit:

`gitlab commit {{project_name}} {{commit_hash}}`

- Get info about jobs in a CI pipeline:

`gitlab pipeline_jobs {{project_name}} {{pipeline_id}}`

- Start a specific CI job:

`gitlab job_play {{project_name}} {{job_id}}`
