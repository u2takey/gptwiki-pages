# authconfig 
## chatgpt 
Linux 命令 authconfig 用于配置系统身份验证，它在系统中设置身份验证的方法和选项。在 Linux 中，身份验证是指用户身份验证，用于校验用户是否有权限访问系统资源。 

一般来说，authconfig 命令主要用于以下方面：

1. 配置本地用户的认证和授权方式，可以选择使用本地密码、LDAP、Kerberos、NIS 等不同的方式进行身份验证；
2. 配置系统的密码策略，如设置最小长度、复杂性要求、过期时间等；
3. 配置 PAM（Pluggable Authentication Modules）模块，这个模块可以扩展 Linux 的身份验证，可以自定义身份验证模块，并且可以适应不同的身份验证需求，如指纹认证等。

下面是一些常用的 authconfig 命令选项：

1. --enableldap：启用 LDAP 认证；
2. --enableldaptls：启用 LDAP 安全传输层协议；
3. --enablekrb5：启用 Kerberos 认证；
4. --enablemkhomedir：如果 LDAP 或 AD 中的用户没有家目录，则在登录时创建家目录；
5. --enablecache：启用 PAM 缓存；
6. --disablecache：禁用 PAM 缓存；
7. --enablepamaccess：启用 PAM 账户访问控制；
8. --enablelocauthorize：启用本地授权。

总之，authconfig 命令是一个非常重要的身份验证工具，在 Linux 服务器中扮演着重要的角色。了解红帽的认证方式和策略管理将有助于管理员灵活地为其 Linux 服务器配置身份验证方案。 

## tldr 
 
> 用于设置系统认证资源的命令行界面。
> 更多信息：<https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/system-level_authentication_guide/authconfig-install>.

- 显示当前的配置（或空运行）：

`authconfig --test`

- 设置服务器使用另一种不同的密码散列算法：

`authconfig --update --passalgo={{算法名}}`

- 启用 LDAP 认证：

`authconfig --update --enableldapauth`

- 关闭 LDAP 认证：

`authconfig --update --disableldapauth`

- 开启网络信息服务（NIS）：

`authconfig --update --enablenis`

- 开启 Kerberos：

`authconfig --update --enablekrb5`

- 开启 Winbind（活动目录）认证：

`authconfig --update --enablewinbindauth`

- 开启本地认证：

`authconfig --update --enablelocauthorize`
