# jarsigner 
## chatgpt 
jarsigner是Java开发者工具包（JDK）中的一个命令行工具，用于对Java扩展库（JAR）和Java包（JAR）进行数字签名。

数字签名可以确保软件的完整性和真实性，它在JAR或JAR文件中插入一个数字签名文件，确保文件在传输或存储过程中没有被篡改或修改。

该命令提供了多个选项，其中包括：

- -keystore：指定包含私钥的密钥库文件的路径
- -storepass：密钥库文件的密码
- -keypass：私钥的密码
- -sigalg：签名算法
- -digestalg：消息摘要算法
- -tsa：时间戳颁发机构的URL

以下命令示例对名为myapp.jar的JAR文件进行数字签名：

jarsigner -keystore mykeystore keystorepass -storepass mypassword myapp.jar alias

这个命令使用名为mykeystore的密钥库文件，包含一个名为alias的条目，它包含需要签名的私钥。还指定了密钥库和密钥的密码。

成功执行命令后，JAR文件将被签名，并在同一个目录下生成一个.signed文件。 

## tldr 
 
> 签名并验证 Java 存档（JAR）文件。
> 更多信息：<https://docs.oracle.com/javase/9/tools/jarsigner.htm>.

- 签名一个 `JAR` 文件：

`jarsigner {{path/to/file.jar}} {{keystore_alias}}`

- 使用特定算法对 `JAR` 文件进行签名：

`jarsigner -sigalg {{algorithm}} {{path/to/file.jar}} {{keystore_alias}}`

- 验证 `JAR` 文件的签名：

`jarsigner -verify {{path/to/file.jar}}`
