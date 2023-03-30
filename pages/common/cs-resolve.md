# cs resolve 
## chatgpt 
As an AI language model, I don't have enough context about the command "cs resolve". But assuming it is a command used in Git version control, it may refer to the following:

In the Git version control system, the "git cherry-pick" command is used to apply a commit from one branch to another. However, sometimes cherry-picking can result in merge conflicts, which need to be resolved before the commit can be applied.

"cs resolve" command may be referring to a custom command or alias set up by the user to resolve conflicts during cherry-picking.

To resolve the conflict, the user needs to open the file in question and manually edit it, resolving the conflicts between the two versions of the file.

Once the user has resolved the conflict and saved the file, they can then complete the cherry-pick operation using the "git cherry-pick --continue" command. This will apply the commit to the new branch and mark it as complete.

So, in summary, "cs resolve" may refer to a custom command or alias set up by the user to resolve conflicts during cherry-picking in the Git version control system. 

## tldr 
 
> Resolve lists the transitive dependencies of one or more other dependencies.
> More information: <https://get-coursier.io/docs/cli-resolve>.

- Resolve lists of transitive dependencies of two dependencies:

`cs resolve {{group_id1}}:{{artifact_id1}}:{{artifact_version1}} {{group_id2}}:{{artifact_id2}}:{{artifact_version2}}`

- Resolve lists of transitive dependencies of a package by the dependency tree:

`cs resolve --tree {{group_id}}:{{artifact_id}}:{{artifact_version}}`

- Resolve dependency tree in a reverse order (from a dependency to its dependencies):

`cs resolve --reverse-tree {{group_id}}:{{artifact_id}}:{{artifact_version}`

- Print all the libraries that depends on a specific library:

`cs resolve {{group_id}}:{{artifact_id}}:{{artifact_version}} --what-depends-on {{searched_group_id}}:{{searched_artifact_id}}`

- Print all the libraries that depends on a specific library version:

`cs resolve {{group_id}}:{{artifact_id}}:{{artifact_version}} --what-depends-on {{searched_group_id}}:{{searched_artifact_id}}{{searched_artifact_version}}`

- Print eventual conflicts between a set of packages:

`cs resolve --conflicts {{group_id1:artifact_id1:artifact_version1 group_id2:artifact_id2:artifact_version2 ...}}`
