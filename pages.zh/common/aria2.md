# aria2 
## chatgpt 
aria2是一款命令行下的多线程下载工具，支持HTTP、FTP、BT等多种协议，具有下载速度快、资源占用少等优点。以下是aria2命令的详细解释：

1. aria2c：启动aria2程序的命令。

2. -s，--split：设置同时下载的线程数。默认值为5。

3. -x，--max-connection-per-server：设置每个服务器的最大连接数。默认值为1。

4. -j，--max-concurrent-downloads：设置最大同时下载任务数。

5. -c，--continue：继续之前的未完成的任务。

6. -i，--input-file：指定下载任务的输入文件，文件中每行包含一个下载链接。

7. -o，--out：设置下载文件的文件名。

8. -d，--dir：设置保存下载文件的路径。

9. --file-allocation：设置磁盘空间分配方式。

10. --max-download-limit：设置最大下载速度，可以限制下载速度以降低带宽消耗。

11. --max-overall-download-limit：设置最大总下载速度，适用于同时下载多个任务的情况。

12. --seed-time：设置BT种子的最小分享时间。

13. --seed-ratio：设置BT种子的分享比率。

14. --bt-stop-timeout：设置BT任务停止的超时时间，单位为秒。

15. --user-agent：设置HTTP请求的User-Agent头。

16. --header：设置HTTP请求头。

17. --referer：设置HTTP请求的Referer头。

18. --save-session：保存下载任务的状态到文件中。

19. --save-session-interval：设置保存下载任务状态的时间间隔，单位为秒。

20. --rpc-listen-port：设置RPC监听端口，用于通过RPC方式控制aria2。

21. --rpc-secret：设置RPC密钥，用于控制访问RPC接口。

以上是aria2命令的详细解释，可以根据自己的需要进行使用。 

## tldr 
 
> 这是 `aria2c` 命令的一个别名。

- 原命令的文档在：

`tldr aria2c`
