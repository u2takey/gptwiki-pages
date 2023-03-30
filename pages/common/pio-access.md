# pio access 
## chatgpt 
Unfortunately, as an AI language model, I do not have enough context to provide a complete answer without more information about what "pio access" refers to. It is possible that "pio" stands for PlatformIO, which is an open-source ecosystem for Internet of Things (IoT) development that supports multiple embedded platforms, and "access" could refer to managing access control and permissions for users to interact with devices or resources within the platform. Without additional context or clarification, it is difficult to provide a more detailed explanation. 

## tldr 
 
> Set the access level on published resources (packages) in the registry.
> More information: <https://docs.platformio.org/en/latest/core/userguide/access/>.

- Grant a user access to a resource:

`pio access grant {{guest|maintainer|admin}} {{username}} {{resource_urn}}`

- Remove a user's access to a resource:

`pio access revoke {{username}} {{resource_urn}}`

- Show all resources that a user or team has access to and the access level:

`pio access list {{username}}`

- Restrict access to a resource to specific users or team members:

`pio access private {{resource_urn}}`

- Allow all users access to a resource:

`pio access public {{resource_urn}}`
