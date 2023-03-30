# airport 
## chatgpt 
airport命令是macOS中的一种命令行工具，主要用于管理和监控Wi-Fi网络连接。以下是该命令一些常见的用法和选项：

- `-s` 或 `--scan`：搜索并列出可用的Wi-Fi网络。
- `-I` 或 `--getinfo`：获取当前Wi-Fi连接的详细信息。
- `-z` 或 `--disassociate`：断开当前Wi-Fi连接。
- `-x` 或 `--xml`：将输出以XML格式呈现。
- `-c` 或 `--channel`：设置Wi-Fi通道号。
- `-h` 或 `--help`：显示命令帮助信息。

使用airport命令可以帮助用户列出可用的Wi-Fi网络、断开当前连接或设置W-Fi通道号等操作。这些操作可以提高用户的网络连接效率和体验。 

## tldr 
 
> 无线网络配置工具。
> 更多信息：<https://ss64.com/osx/airport.html>.

- 显示当前的无线状态信息：

`airport -I`

- 在通道 1 上监察（嗅探）无线流量：

`airport sniff {{1}}`

- 扫描可用的无线网络：

`airport -s`

- 与当前的 Airport 网络脱离连接：

`sudo airport -z`
