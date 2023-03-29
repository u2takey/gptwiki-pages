# clamav 
## chatgpt 
ClamAV是一款免费的开源杀毒软件，可用于检测恶意软件或病毒。以下是ClamAV常用的命令和其作用：

1. clamscan：用于扫描文件、文件夹或整个系统以检测恶意软件。

2. freshclam：用于更新ClamAV病毒数据库，以确保最新的病毒定义可以检测到新出现的病毒。

3. clamd：ClamAV守护进程，用于实时监测文件，以及在系统启动时自动启动ClamAV服务。

4. clamdscan：与clamscan类似，但是使用ClamAV守护进程进行扫描，可以提高性能，并且支持在文件扫描中排除某些目录或特定类型的文件。

5. clamconf：用于查看和编辑ClamAV配置文件，例如定义扫描选项，设置扫描时排除文件和目录等。

6. freshclam.conf：ClamAV自动更新病毒数据库的配置文件。在此文件中，可以定义更新源和更新频率。

7. clamd.conf：配置ClamAV守护进程的配置文件。可以在此文件中定义ClamAV的限制、扫描选项、日志设置等。 

## tldr 
 
> 这是 `clamdscan` 命令的一个别名。
> 更多信息：<https://www.clamav.net>.

- 原命令的文档在：

`tldr clamdscan`
