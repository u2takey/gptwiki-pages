# airodump-ng 
## chatgpt 
airodump-ng 是一个用于 Wi-Fi 网络的嗅探和分析工具。该工具可以在监视模式下探测无线网络并显示有关其身份，信道，安全性等方面的详细信息。它支持多种输出格式，如 pcap，CSV，XML，Kismet log 等。

命令 airodump-ng 用于启动 airodump-ng 工具，并开始监听无线网络。该命令后面可以跟一些参数来指定要监视的网络和其它选项。例如：

`airodump-ng wlan0` - 在 wlan0 网卡上启动 airodump-ng 并监听所有可见无线网络。

`airodump-ng --bssid 00:11:22:33:44:55 -c 6 wlan0` - 在 wlan0 网卡上，只监听以 MAC 地址 00:11:22:33:44:55 的访问点，并将其设为信道6。

`airodump-ng --write out --output-format csv wlan0` - 在 wlan0 网卡上启动 airodump-ng 并将所有数据记录到名为 out.csv 的 CSV 文件。

总之，airodump-ng 工具是一种非常强大的网络嗅探工具，可以帮助您了解无线网络的实际情况，以便进行安全分析或优化网络性能。 

## tldr 
 
> 捕获数据包并显示有关无线网络的信息。
> `aircrack-ng` 的一部分。
> 更多信息： <https://www.aircrack-ng.org/doku.php?id=airodump-ng>.

- 捕获数据包并显示有关无线网络的信息：

`sudo airodump-ng {{interface}}`

- 捕获数据包并显示有关无线网络的信息，给定 MAC 地址和信道，并将输出保存到文件中：

`sudo airodump-ng --channel {{信道}} --write {{路径/到/文件}} --bssid {{mac}} {{interface}}`
