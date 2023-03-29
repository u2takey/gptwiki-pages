# amass 
## chatgpt 
amass是一个扫描互联网资产的工具，它有多种用途，如发现域名、主机、端口等。amass可以从多个来源获取信息，包括结构化和非结构化的数据来源。该工具可以与其他扫描工具（如nmap）配合使用，可以生成结果报告，并支持各种输出格式（如JSON和CSV）。

以下是amass一些常用的命令和参数：

1. 扫描域名: amass enum -d example.com

此命令将扫描“example.com”域名，找到与其相关的子域名。

2. 指定扫描源: amass enum -d example.com -src

此命令将扫描"example.com"域名，并指定采用"源"作为扫描源，"源"可以是SHODAN或Censys等。

3. 指定端口扫描: amass enum -d example.com -p 80,443

此命令将扫描"example.com"域名，并指定只扫描80和443端口。

4. 扫描IP地址: amass intel -addr 8.8.8.8

此命令将扫描8.8.8.8地址，查找与该IP关联的域名和子域名。

5. 生成报告: amass enum -d example.com -json outfile.json

此命令将扫描"example.com"域名，并将结果保存为JSON格式的文件"outfile.json"。

总之，amass是一个功能强大的扫描工具，可用于发现互联网上的资产，支持多种输出格式，适用于渗透测试、红队操作和其他安全测试工作。 

## tldr 
 
> 深度攻击面探测与资产发现工具。
> 此命令也有关于其子命令的文件，例如：`amass db`.
> 更多信息：<https://github.com/OWASP/Amass>.

- 执行 Amass 子命令：

`amass {{子命令}}`

- 展示帮助信息：

`amass -help`

- 展示子命令帮助信息（如 `intel`、`enum` 等）：

`amass -help {{子命令}}`

- 查看 Amass 版本：

`amass -version`
