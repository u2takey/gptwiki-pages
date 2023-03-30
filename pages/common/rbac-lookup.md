# rbac-lookup 
## chatgpt 
As an AI language model, I can describe what RBAC means and what the possible meanings of `rbac-lookup` could be in different contexts.

RBAC stands for Role-based Access Control, which is a security model that provides access control based on the roles assigned to users or groups in a system. A role-based access control system defines roles based on job functions within an organization and restricts user access to authorized roles.

The command `rbac-lookup` could have different meanings depending on the context in which it is used. Here are a few possibilities:

1. In Kubernetes cluster administration, `rbac-lookup` might be a command-line tool used to verify the permissions of users or service accounts in a Kubernetes cluster. This tool could display the effective roles, role bindings, and access control list (ACL) rules based on RBAC policies.

2. In the context of network and security management, `rbac-lookup` might be a tool used to lookup access rules defined by a Role-Based Access Control (RBAC) system. This tool could provide information on different access levels (admin, user, guest, etc.) and access rights based on defined policies.

3. `rbac-lookup` could also be used in software development to look up user permissions and roles based on RBAC policies. This could help developers ensure that users have the correct level of permissions and access in the application.

Overall, the meaning and usage of `rbac-lookup` can vary depending on the context in which it is used. It is important to understand the specific use case and environment before using this command. 

## tldr 
 
> Find roles and cluster roles attached to any user, service account or group name in your Kubernetes cluster.
> More information: <https://github.com/reactiveops/rbac-lookup>.

- View all RBAC bindings:

`rbac-lookup`

- View RBAC bindings that match a given expression:

`rbac-lookup {{search_term}}`

- View all RBAC bindings along with the source role binding:

`rbac-lookup -o wide`

- View all RBAC bindings filtered by subject:

`rbac-lookup -k {{user|group|serviceaccount}}`

- View all RBAC bindings along with IAM roles (if you are using GKE):

`rbac-lookup --gke`
