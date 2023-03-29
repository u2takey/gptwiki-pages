# heroku 
## chatgpt 
heroku 命令是一个命令行工具，用于与 Heroku 云服务平台交互。通过 heroku 命令，用户可以管理 Heroku 上的应用、部署代码、管理数据库、查看日志等。具体命令包括：

1. heroku create: 创建一个新的 Heroku 应用。
2. heroku apps: 列出用户拥有的所有应用。
3. heroku logs: 查看应用的日志。
4. heroku open: 打开一个应用的网页。
5. heroku ps: 查看应用的进程状态。
6. heroku config: 管理应用的配置变量。
7. heroku addons: 管理应用的插件。
8. heroku run: 在应用运行一个命令。
9. heroku git: 管理应用的 Git 仓库。
10. heroku buildpacks: 管理应用的构建插件。

通过 heroku 命令，用户可以轻松管理自己的应用，快速部署代码并监控应用。 

## tldr 
 
> 从命令行创建和管理 Heroku 应用。
> 更多信息：<https://www.heroku.com/>.

- 登录到你的 heroku 帐户：

`heroku login`

- 创建一个 heroku 应用：

`heroku create`

- 显示应用的日志：

`heroku logs --app {{app_name}}`

- 在 dyno（Heroku 虚拟机）中运行一次性进程：

`heroku run {{process_name}} --app {{app_name}}`

- 列出应用的 dyno（Heroku 虚拟机）：

`heroku ps --app {{app_name}}`

- 永久销毁应用：

`heroku destroy --app {{app_name}}`
