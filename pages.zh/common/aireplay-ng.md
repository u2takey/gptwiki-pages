# aireplay-ng 
## chatgpt 
aireplay-ng是aircrack-ng套件中的一个成员，主要用于无线网络的攻击和测试。该命令提供了一系列攻击选项，包括：

1.攻击“认证”过程：此选项可强制客户端重新认证，从而使攻击者能够捕获诸如WEP、WPA等密码。

2.攻击“重连”过程：此选项用于断开客户端与接入点之间的连接，从而迫使客户端重新连接，并提供一个机会来捕获密码。

3.攻击“注入”数据包：此选项创建重复包，并将其注入到连接中，以误导网络身份验证交换。

4.攻击“组密码”：这将与一个特定的MAC地址或所有MAC进行连接。它还可以扫描网络以查找此MAC地址。

总之，aireplay-ng提供了各种工具和技术，可帮助安全测试人员评估无线网络的安全状况，并帮助攻击者破解密码。因此，使用此命令需要谨慎，需要遵守法律和伦理规范。 

## tldr 
 
> 向无线网络注入数据包。
> `aircrack-ng` 的一部分。
> 更多信息：<https://www.aircrack-ng.org/doku.php?id=aireplay-ng>.

- 向指定的接入点（AP）MAC 地址、客户端 MAC 地址和接口发送指定数量的去关联（disassociate）数据包：

`sudo aireplay-ng --deauth {{count}} --bssid {{ap_mac}} --dmac {{client_mac}} {{interface}}`
