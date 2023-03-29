# bpftrace 
## chatgpt 
bpftrace是一种基于eBPF（extended Berkeley Packet Filter）的针对Linux系统的高级跨平台的动态跟踪工具。它允许系统管理员和开发人员可以以简便灵活的方式来分析操作系统的运行情况。 下面是bpftrace命令及其用途的详细解释：

1. bpftrace -e 'probe:netdev { print(arg0) }'
   - 用于监测网络设备上发生的事件，并打印设备信息。

2. bpftrace -e 'tracepoint:syscalls:sys_enter_open { printf("%s %s\n", comm, str(args->filename->data)); }'
   - 用于跟踪系统调用（syscall）中的open函数，并打印调用者和文件名信息。

3. bpftrace -e 'kprobe:do_sys_open { printf("%s\n", ustring(@filename)); }'
   - 用于跟踪do_sys_open内核函数，并打印其调用参数信息。

4. bpftrace -e 'tracepoint:sched:sched_switch { printf("%d %s -> %s\n", pid, comm, arg2); }'
   - 用于跟踪调度器事件，并打印进程ID、进程名以及状态信息。

5. bpftrace -e 'uprobe:/lib/x86_64-linux-gnu/libc.so.6:read { printf("%s\n", ustring($arg1)); }'
   - 用于跟踪libc库中的read函数，并打印其调用参数信息。

总之，bpftrace命令是一种强大的动态跟踪工具，可以帮助Linux系统管理员和开发人员通过灵活的命令来监控和分析系统运行情况，从而解决相关问题。 

## tldr 
 
> Linux eBPF 的高级跟踪语言。
> 更多信息：<https://github.com/iovisor/bpftrace>.

- 显示 bpftrace 版本：

`bpftrace -V`

- 列出所有可用的探针：

`sudo bpftrace -l`

- 运行单行程序（例如按程序进行系统调用计数）：

`sudo bpftrace -e '{{tracepoint:raw_syscalls:sys_enter { @[comm] = count(); }}}'`

- 从文件运行程序：

`sudo bpftrace {{文件}}`

- 通过 PID 跟踪程序：

`sudo bpftrace -e '{{tracepoint:raw_syscalls:sys_enter /pid == 123/ { @[comm] = count(); }}}'`

- 进行试运行并以 eBPF 格式显示输出：

`sudo bpftrace -d -e '{{单行程序}}'`
