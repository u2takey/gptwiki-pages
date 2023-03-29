# jenv 
## chatgpt 
jenv是一个Java版本管理工具，用于在多个Java版本之间进行切换。使用jenv，用户可以轻松安装和管理多个Java版本。下面是jenv命令的详细说明：

1. jenv versions：列出当前所有已安装的Java版本。

2. jenv global [version]：设置全局的Java版本。如果不带参数，则显示当前设置的全局版本。

3. jenv local [version]：在当前目录下设置Java版本。如果不带参数，则显示当前目录下设置的Java版本。

4. jenv shell [version]：在当前shell中设置Java版本。如果不带参数，则显示当前shell中设置的Java版本。

5. jenv install [version]：安装指定版本的Java。

6. jenv uninstall [version]：卸载指定版本的Java。

7. jenv version ：显示当前jenv版本。

8. jenv rehash：重置jenv的路径缓存。

9. jenv doctor：检查系统配置是否正确。

10. jenv enable-plugin [plugin-name]：启用指定的插件。

11. jenv disable-plugin [plugin-name]：禁用指定的插件。

总之，jenv提供了一个简单而灵活的方式来管理Java版本。用户可以很容易地安装、卸载和切换不同版本的Java。 

## tldr 
 
> 管理”JAVA_HOME“环境变量的命令行工具。
> 更多信息：<https://www.jenv.be/>.

- 向 jEnv 添加一个 Java 版本：

`jenv add {{Java Home 路径}}`

- 显示当前使用的 JDK 版本：

`jenv version`

- 显示所有托管的 JDK：

`jenv versions`

- 设置全局JDK版本：

`jenv global {{Java 版本}}`

- 设置当前 shell 会话的 JDK 版本：

`jenv shell {{Java 版本}}`

- 启用 jEnv 插件：

`jenv enable-plugin {{插件名称}}`
