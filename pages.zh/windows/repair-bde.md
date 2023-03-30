# repair-bde 
## chatgpt 
repair-bde是一个Windows命令行工具，用于修复或解密BitLocker加密的驱动器。它是BitLocker驱动器加密（BDE）管理器的一部分，并且需要管理员特权才能运行。

该命令有多个可选参数：

- -ForceDismount：强制解除BitLocker加密
- -FirmwareTest：检查BitLocker固件兼容性
- -KeyFilePath：指定解密密钥所在的路径
- -RecoveryPassword：指定恢复密码
- -RecoveryKey：指定恢复密钥
- -SkipHardwareTest：跳过对硬件的兼容性测试
- -UseRecoveryPassword：使用恢复密码进行解密
- -Verbose：提供更详细的输出

例如，如果您想尝试从指定的密钥文件解密驱动器并跳过硬件测试：

repair-bde C: D: -KeyFilePath "C:\BitLockerKeys\MyBitLockerKey.bek" -SkipHardwareTest

该命令会将C盘上的BitLocker加密驱动器解密到D盘，使用指定的密钥文件，并跳过硬件兼容性测试。请注意，解密BitLocker驱动器需要相应的密钥或密码，否则该命令无法工作。 

## tldr 
 
> 尝试修复或解密损坏的 BitLocker 加密卷。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/repair-bde>.

- 尝试修复一个指定的卷：

`repair-bde {{C:}}`

- 尝试修复指定的卷并输出到另一个卷：

`repair-bde {{C:}} {{D:}}`

- 尝试使用提供的恢复密钥文件修复指定的卷：

`repair-bde {{C:}} -RecoveryKey {{bek 文件的路径}}`

- 尝试使用提供的数字恢复密码修复指定的卷：

`repair-bde {{C:}} -RecoveryPassword {{密码}}`

- 尝试使用提供的密码修复指定的卷：

`repair-bde {{C:}} -Password {{密码}}`

- 尝试使用提供的密钥包修复指定的卷：

`repair-bde {{C:}} -KeyPackage {{目录的路径}}`

- 将日志输出到指定的文件：

`repair-bde {{C:}} -LogFile {{文件的路径}}`

- 显示所有可用的选项：

`repair-bde /?`
