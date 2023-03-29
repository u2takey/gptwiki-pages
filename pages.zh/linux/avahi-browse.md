# avahi-browse 
## chatgpt 
avahi-browse 是一个 Linux 命令，用于在本地网络上扫描服务或服务类型。它是 Avahi 系统工具之一，它是一种自动网络服务发现程序，可让用户发现其他计算机和设备上的服务和设备。Avahi 帮助用户轻松地发现其他计算机和设备上可用的网络服务和资源。

使用 avahi-browse 命令可以查找：

- 服务：它可以搜索网络上的所有可用服务，例如打印机、文件共享、Web 服务器等。
- 服务类型：它可以列出当前在网络上可用的所有服务类型，例如 SSH、HTTP 和 FTP。

Avahi-browse 还可以列出每个服务的 IP 地址、端口号、服务名和服务器类型等详细信息，以便更轻松地访问这些服务。

下面是使用 avahi-browse 命令的基本语法：

```
avahi-browse [OPTIONS] [SERVICE_TYPE]
```

参数说明：

- OPTIONS：支持的选项，例如 -a 表示列出所有可用服务，-t 表示列出特定类型的所有服务。
- SERVICE_TYPE：要搜索的服务类型，例如 _http._tcp 表示搜索 HTTP 服务。

例如，以下命令将列出所有可用的 HTTP 服务：

```
avahi-browse -t _http._tcp
```

这将输出所有可用的 HTTP 服务和它们的详细信息，例如服务名、IP 地址和端口号等。

总之，avahi-browse 命令可以帮助用户发现网络上的可用服务和资源，从而更轻松地访问这些服务。 

## tldr 
 
> 显示通过 mDNS/DNS-SD 暴露在本地网络的服务和主机。
> Avahi 与苹果设备的 Bonjour（Zeroconf）兼容。
> 更多信息：<https://www.avahi.org/>.

- 列出本地网络中的所有服务和他们的地址与端口，忽略他们本地的地址和端口：

`avahi-browse --all --resolve --ignore-local`

- 列出所有的域名：

`avahi-browse --browse-domains`

- 只搜索一个特定的域名：

`avahi-browse --all --domain={{domain}}`
