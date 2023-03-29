# chage 
## chatgpt 
chage 是一个 Linux 命令，用于更改用户密码的过期时间。当用户密码过期时，系统会在用户登录时提示用户更改密码。

该命令的基本语法为：

```
chage [options] LOGIN
```

其中，LOGIN 是要更改密码过期时间的用户的登录名。

选项包括：

- `-d, --lastday LAST_DAY`: 设置密码的最后一天。该选项采用 YYYY-MM-DD 格式的日期。
- `-E, --expiredate EXPIRE_DATE`: 设置密码的过期时间。该选项采用 YYYY-MM-DD 格式的日期。
- `-m, --mindays MIN_DAYS`: 设置更改密码之间的最小天数间隔。
- `-M, --maxdays MAX_DAYS`: 设置密码过期的最大天数间隔。
- `-I, --inactive INACTIVE`: 设置账户失效的天数。如果账户在该天数内未被使用，账户将被锁定。
- `-W, --warndays WARN_DAYS`: 设置在密码过期之前多少天开始提醒用户更改密码。

例如，要将用户 johndoe 的密码最小间隔设置为 7 天，最大间隔设置为 60 天，可以使用以下命令：

```
chage -m 7 -M 60 johndoe
```

更改用户密码过期日期的命令示例：

```
chage -E 2023-01-01 johndoe
```

这将改变用户 johndoe 的密码过期日期为 2023 年 1 月 1 日。 

## tldr 
 
> 更改用户账户和密码到期信息。
> 更多信息：<https://manned.org/chage>.

- 列出用户的密码信息：

`chage --list {{用户名}}`

- 启用密码在 10 天内过期：

`sudo chage --maxdays {{10}} {{用户名}}`

- 关闭密码过期：

`sudo chage --maxdays {{-1}} {{用户名}}`

- 设置账户到期日期：

`sudo chage --expiredate {{YYYY-MM-DD}} {{用户名}}`

- 强制用户在下次登录时更改密码：

`sudo chage --lastday {{0}} {{用户名}}`
