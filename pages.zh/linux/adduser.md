# adduser 
## chatgpt 
adduser 命令用于在 Linux 系统中创建新用户账号。在运行该命令时，可以指定要创建的新用户的用户名、密码、UID（用户标识号码）、GID（组标识号码）、家目录、姓名等信息。如果没有指定这些信息，adduser 会使用默认设置来创建新用户账号。

adduser 命令通常需要以 root 用户或具有 sudo 权限的用户身份运行。运行 adduser 命令后，系统会提示您输入新用户的密码和确认密码。然后，系统会自动创建新的用户账号并创建相应的家目录。通过创建新用户账号，您可以为新用户提供独立的登录和权限，以满足各种安全和管理需求。

以下是 adduser 命令的一些常用选项和参数：

- --home 目录：指定新用户的家目录。
- --shell shell：指定新用户的默认 shell。
- --ingroup 组名：将新用户添加到指定的用户组。
- --disabled-login：创建一个不能登录系统的用户账号。
- --system：创建一个系统账户，适用于运行某些服务的用户账号。
- --gecos 信息：指定用于新用户的 GECOS 信息（包含有关该用户的其他详细信息）。

以下是一个实际的 adduser 命令示例：

sudo adduser testuser --home /mnt/data --ingroup users

上述命令将创建一个名为 testuser 的新用户账号，并将其添加到 users 组中。该用户的家目录将被设置为 /mnt/data 目录。 

## tldr 
 
> 添加用户的工具。
> 更多信息：<https://manpages.debian.org/latest/adduser/adduser.html>.

- 创建一个新用户，在默认路径创建 home 目录，并提示用户设置密码：

`adduser {{用户名}}`

- 创建一个新用户，不生成 home 目录：

`adduser --no-create-home {{用户名}}`

- 创建一个新用户，并在指定路径下创建 home 目录：

`adduser --home {{home 路径}} {{用户名}}`

- 创建一个新用户，并指定登录 shell：

`adduser --shell {{shell 路径}} {{用户名}}`

- 创建一个新用户，并指定其用户组：

`adduser --ingroup {{用户组}} {{用户名}}`
