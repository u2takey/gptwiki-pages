# md5sum 
## chatgpt 
md5sum命令是一个用于计算并显示文件MD5摘要的命令行程序。MD5（Message-Digest Algorithm 5）是一个在密码学和计算机安全领域中广泛使用的哈希函数，它将任意长度的输入数据产生一个128位的散列值。md5sum命令可用于验证文件内容是否相同。当一个文件的MD5散列与已知正确的散列相匹配时，可以确定该文件不具有篡改或其他修改。

md5sum命令的基本语法如下：

md5sum [File]

其中，[File]是要计算其MD5散列的文件名。默认情况下，md5sum会打印出文件的MD5散列值和文件名，以便后续进行比较和验证。

例如，以下命令将计算名为"file.txt"的文件的MD5散列：

md5sum file.txt

输出结果将类似于：

5d41402abc4b2a76b9719d911017c592  file.txt

这表示该文件的MD5散列为"5d41402abc4b2a76b9719d911017c592"。如果该命令输出值与另一个文件或来源提供的MD5散列值相匹配，则可以确定文件内容没有被修改或损坏。 

## tldr 
 
> 计算 MD5 加密校验和。
> 更多信息：<https://www.gnu.org/software/coreutils/md5sum>.

- 计算文件的 MD5 校验和：

`md5sum {{path/to/file}}`

- 计算多个文件的 MD5 校验和：

`md5sum {{path/to/file1}} {{path/to/file2}}`

- 读取 MD5SUM 的文件并验证所有文件是否具有匹配的校验和：

`md5sum -c {{path/to/file.md5}}`
